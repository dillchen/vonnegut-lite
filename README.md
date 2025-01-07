# Vonnegut Lite

A lightweight version of Vonnegut that uses Cursor's AI capabilities to help write your novel. This version doesn't require any dependencies or setup - just Cursor and these prompts.

## Getting Started

1. Create a new directory for your novel
2. Copy this entire `/lite` directory into it
3. Create a `story-seed.json` file based on `seed.example.json`
4. Create the following directory structure:
```
your-novel/
├── Background/          # Story background and metadata
├── Chapter-1/          # First chapter
│   ├── scenes/         # Scene files
│   ├── drafts/         # Draft files
│   ├── critiques/      # Critique files
│   └───| additions/      # New story elements
│       ├── characters/ # New characters
│       ├── settings/   # New locations
│       └── plot-points/# New plot elements
└── lite/               # This directory
    └── prompts/        # AI prompts for each step
```

## How to Use

Each command from the original Vonnegut has been converted to a markdown file in the `prompts` directory. To use them:

1. Open the relevant prompt file in Cursor
2. Follow the instructions at the top of the file
3. Use Cursor's AI to execute the prompts against your content
4. Save the generated content in the appropriate directory

### Command Order

Typical workflow for each chapter:

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