# Draft Generation Prompt

Use this prompt with Cursor's AI to generate chapter drafts from your scenes.

## Process Overview

1. Read all scenes from the chapter's scenes directory
2. Generate initial draft in sections (max 1000 words per section)
3. Expand draft if under minimum length
4. Clean and format the final draft

## Word Count Targets

- Minimum: 3,500 words
- Maximum: 4,500 words
- Section Target: 1,500 words
- Chunk Size: ~500 words

## Instructions

1. **Preparation**
   - Ensure all scenes are written and numbered (scene-1.md, scene-2.md, etc.)
   - Have your scenes open in Cursor
   - Create a new file for the draft in the drafts directory

2. **Initial Draft Generation**
   Use this prompt for each section (copy scenes content where indicated):
   ```
   Based on these scenes:

   [PASTE SCENES HERE]

   Please generate this section of the chapter draft. This is section [N] of [TOTAL].
    
   Requirements:
   1. [If first section: Start with "Chapter X:" followed by a title and a strong hook]
      [If not first: Continue smoothly from the previous section]
   2. Maintain consistent narrative voice and perspective
   3. Use "* * *" for scene breaks between major scenes
   4. Focus on character development, sensory details, and vivid descriptions
   5. Keep the narrative focused and avoid tangents
   6. Ensure smooth transitions between scenes

   Previous content (for context):
   [PASTE LAST 300 WORDS OF PREVIOUS SECTION IF NOT FIRST]

   Following content (for context):
   [PASTE FIRST 300 WORDS OF NEXT SECTION IF NOT LAST]
   ```

3. **Expansion Prompt**
   If the draft is under 3,500 words, use this prompt for each section:
   ```
   Please expand this text by adding approximately [TARGET] words:

   [PASTE SECTION HERE]

   Requirements:
   1. Keep ALL existing content exactly as is
   2. Add exactly [TARGET] new words through additional details
   3. DO NOT rewrite or remove anything
   4. Add vivid sensory details
   5. Deepen character emotions
   6. Enhance the atmosphere
   7. Add meaningful dialogue
   8. Maintain the style
   9. Focus on quality while adding words
   ```

4. **Retry Prompt**
   If a section fails or needs improvement:
   ```
   Please continue the story based on these scenes:

   [PASTE SCENES HERE]

   Previous scenes:
   [PASTE PREVIOUS SECTION SCENES]

   Following scenes:
   [PASTE NEXT SECTION SCENES]

   Requirements:
   1. Keep it simple and focused
   2. Maintain the same narrative voice
   3. Connect smoothly with both the previous and following content
   4. Focus on the key events and character moments
   ```

## Best Practices

1. **Section Processing**
   - Process 2-3 scenes per section
   - Check word count after each section
   - Ensure smooth transitions between sections
   - Maintain consistent style and voice

2. **Content Cleanup**
   - Remove any meta-commentary or instructions
   - Format scene breaks consistently
   - Check chapter number and title
   - Normalize paragraph spacing

3. **Quality Checks**
   - Verify narrative continuity
   - Check character consistency
   - Ensure all scenes are included
   - Validate dialogue formatting

4. **File Management**
   - Save draft as `draft-N.md` (where N is the next number)
   - Include descriptive suffix (e.g., `draft-1-expanded.md`)
   - Keep all versions for reference
   - Update `index.md` with final version

## Troubleshooting

1. **If Section Generation Fails**
   - Try with fewer scenes per section
   - Use the retry prompt
   - Break into smaller chunks
   - Focus on key events only

2. **If Expansion Needed**
   - Start with smaller word targets
   - Focus on one aspect at a time
   - Use multiple expansion passes
   - Verify quality between passes

3. **If Style Inconsistent**
   - Review story seed style guide
   - Check previous chapters
   - Use style-specific prompts
   - Manual editing may be needed

## Example Workflow

1. **Initial Setup**
   ```bash
   # Create draft file
   touch Chapter-1/drafts/draft-1-initial.md
   ```

2. **Section Generation**
   - Copy scenes into groups
   - Apply section prompt
   - Save each section
   - Check transitions

3. **Expansion (if needed)**
   - Calculate words needed
   - Split into chunks
   - Apply expansion prompt
   - Combine and check

4. **Cleanup and Save**
   - Remove artifacts
   - Format consistently
   - Update index
   - Save final version

## Notes

- Keep track of word count manually
- Save frequently
- Review each section before proceeding
- Maintain consistent formatting
- Check for content overlap
- Ensure proper scene breaks
- Verify chapter formatting 