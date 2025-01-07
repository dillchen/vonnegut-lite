# Vonnegut Lite

A lightweight version of Vonnegut that uses Cursor's AI capabilities to help write your novel. This version doesn't require any dependencies or setup - just Cursor and these prompts.

> "There is no reason why the simple shapes of stories can't be fed into computers. They are beautiful shapes."  
> -- Kurt Vonnegut

[Watch Kurt Vonnegut on the "Shape of Stories" on YouTube](https://www.youtube.com/watch?v=GOGru_4z1Vc)

Based on Vonnegut's observation, and leveraging this project's prompt flow, we can start from a simple story seed and systematically build out a fully fleshed novel—one chapter at a time.

## Quick Start with Cursor

1. **Get the Starter Repo**:
```bash
# Fork this repo on GitHub, then clone to your desktop
git clone https://github.com/YOUR_USERNAME/vonnegut-lite.git
cd vonnegut-lite

# Or clone directly (if you don't plan to contribute back)
git clone https://github.com/commonxyz/vonnegut-lite.git
cd vonnegut-lite
```

2. **Enable Cursor Features**:
```bash
# Open Cursor's Command Palette
Cmd/Ctrl + Shift + P

# Enable Composer Mode
Type: "Enable Composer Mode (with Agentic Mode)"

# (Optional) Enable Yolo Mode for more direct file creation
Type: "(Optional) Enable Yolo Mode"
```

3. **Initialize Your Novel**:
```bash
# Copy this into Cursor's Composer:
"Create a new novel project with the following:
- Create a 'novel' directory
- Set up all required subdirectories
- Initialize story-seed.json and checklist.json from examples
- Prepare the first chapter structure"
```

## Prompt Flow Loop

The writing process follows a cyclical pattern of prompts, each building upon the previous step:

1. **Expand** (Run Once)
   - Initial story expansion
   - Develop core concepts
   - Create detailed character profiles
   - Build world and setting details
   - Set up story structure

2. **Plan** (Each Writing Session)
   - Review previous content
   - Outline next scene/chapter
   - Set specific goals
   - Identify key story beats

3. **Research** (Optional)
   - Gather necessary background information
   - Verify technical details
   - Study similar works for inspiration
   - Document findings for reference

4. **Act**
   - Write character dialogue
   - Create scene descriptions
   - Develop action sequences
   - Build emotional moments

5. **Draft**
   - Combine scene elements
   - Write connecting passages
   - Add descriptive details
   - Ensure flow and pacing

6. **Critique**
   - Review for consistency
   - Check character voices
   - Analyze pacing
   - Identify weak points
   - Suggest improvements

7. **Revise**
   - Address critique points
   - Strengthen weak areas
   - Polish prose
   - Enhance descriptions
   - Tighten dialogue

Return to Step 2 (Plan) for the next scene/chapter.

### Using the Loop

- Start each writing session at Step 2 (Plan)
- Complete steps 2-7 for each scene/chapter
- Use Research (Step 3) as needed
- Track progress in checklist.json
- Save work after each step
- Review previous work before planning next section

## Manual Setup (Alternative)

If you prefer to set up manually, run these commands:
```bash
# Create project structure
mkdir novel
cd novel

# Create required directories
mkdir -p background/research
mkdir -p chapter-1/{scenes,drafts,critiques}
mkdir -p chapter-1/additions/{characters,settings,plot-points}

# Initialize tracking files
cp ../seed.example.json story-seed.json
cp ../checklist.example.json checklist.json
```

Your directory structure should look like this:
```
.                      # Root directory
├── prompts/          # AI prompts directory
│   ├── act.md
│   ├── critique.md
│   ├── draft.md
│   ├── plan.md
│   ├── research.md
│   └── revise.md
├── novel/            # Your novel directory
│   ├── background/   # Story background and metadata
│   │   └── research/# Research documents
│   ├── chapter-1/   # First chapter
│   │   ├── scenes/  # Scene files
│   │   ├── drafts/  # Draft files
│   │   ├── critiques/ # Critique files
│   │   └── additions/ # New story elements
│   │       ├── characters/
│   │       ├── settings/
│   │       └── plot-points/
│   ├── story-seed.json  # Story configuration
│   └── checklist.json   # Progress tracking
├── seed.example.json    # Template for story-seed.json
└── checklist.example.json # Template for checklist.json
```

## Instructions for Cursor Composer

1. Navigate to your project:
```bash
cd novel
```

2. Use Composer (Cmd/Ctrl + Shift + P) to:
   - Generate content based on prompts
   - Analyze existing content
   - Track progress through checklist
   - Manage file creation

3. For each prompt file:
   - Open the relevant `.md` file from `../prompts/`
   - Select the appropriate prompt section
   - Use Composer to execute the prompt
   - Save generated content in the correct directory:
     ```bash
     # Example: Creating a new scene
     touch chapter-1/scenes/scene-1.md
     
     # Example: Creating a draft
     touch chapter-1/drafts/draft-1.md
     ```

4. Track Progress:
   ```bash
   # Open checklist in Cursor
   open checklist.json
   
   # Update task status and timestamp when complete
   ```

### Command Order

The `checklist.json` file enforces this workflow for each chapter:

1. `plan.md` - Plan the chapter structure
2. `research.md` - Generate background information
3. `act.md` - Create scenes and dialogue
4. `draft.md` - Generate chapter draft
5. `critique.md` - Review and analyze content
6. `revise.md` - Update draft based on critiques

### Word Count Targets

- Chapter minimum: 3,500 words
- Chapter maximum: 4,500 words
- Scene target: ~1,000 words
- Section target: ~1,500 words

## Story Seed

The `seed.example.json` file provides the template for your story's initial configuration. Copy it to `story-seed.json` and customize:

- Title and concept
- Main characters
- Key settings
- Major plot points
- Themes and tone

## Tips for Using with Cursor

1. Keep the relevant prompt file open while working
2. Use Cursor's AI to:
   - Generate content based on prompts
   - Analyze existing content
   - Suggest improvements
   - Help with transitions
   - Check for consistency

3. Save generated content immediately
4. Review and edit AI output before proceeding
5. Keep track of word counts manually
6. Maintain consistent file naming:
   - Scenes: `scene-1.md`, `scene-2.md`, etc.
   - Drafts: `draft-1.md`, `draft-2.md`, etc.
   - Critiques: `critique-1.md`, `summary-1.md`, etc.

## Best Practices

1. **Scene Writing**
   - One major event per scene
   - Include character development
   - Balance dialogue and description
   - Maintain consistent POV

2. **Drafting**
   - Generate in sections (~1000 words each)
   - Check transitions between sections
   - Ensure consistent voice
   - Track word count

3. **Critiquing**
   - Check technical accuracy
   - Verify character consistency
   - Review plot progression
   - Assess pacing and flow

4. **Revising**
   - Address all critique points
   - Maintain narrative flow
   - Check for continuity
   - Polish prose style

## Directory Structure Details

### Background/
- `outline.md` - Full story outline
- `characters.md` - Character profiles
- `settings.md` - Location descriptions
- `timeline.md` - Story timeline
- `research.md` - Background research

### Chapter-N/
- `scenes/` - Individual scene files
- `drafts/` - Chapter drafts
- `critiques/` - Review feedback
- `additions/` - New story elements

### Additions Tracking

Track new story elements in each chapter's `additions` directory:

1. **Characters**
   - Name and role
   - Introduction context
   - Development potential

2. **Settings**
   - Location details
   - Atmospheric elements
   - Story significance

3. **Plot Points**
   - Event description
   - Connection to main plot
   - Future implications

## Error Recovery

If Cursor's AI gives unexpected results:

1. Break the task into smaller chunks
2. Provide more specific context
3. Rephrase the prompt
4. Try alternative approaches from the prompt file
5. Review and manually edit if needed

## Contributing

Feel free to improve these prompts and share your experiences. Create issues or pull requests on the GitHub repository.

## Using the Checklist

The `checklist.example.json` file provides a template for tracking progress:

1. **Structure**
   - Tasks are grouped by scope (background, chapter-N)
   - Each task has dependencies and completion status
   - Timestamps track when tasks are completed

2. **Task Flow**
   - Complete tasks in dependency order
   - Mark tasks complete in checklist
   - Use timestamps for progress tracking

3. **Managing with Cursor**
   - Open checklist.json in Cursor
   - Update status as tasks complete
   - Use Composer to validate progress
   - Track dependencies automatically 