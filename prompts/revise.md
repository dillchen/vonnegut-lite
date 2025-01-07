# Revision Prompt

Use this prompt with Cursor's AI to revise chapter drafts based on critiques.

## Process Overview

1. Read the latest draft and all critiques
2. Create a revision plan based on critique priorities
3. Process the draft in sections with focused improvements
4. Verify length and quality requirements
5. Save the revised version

## Word Count Targets

- Minimum: 3,500 words
- Maximum: 4,500 words
- Section Size: ~1,000 words

## Instructions

1. **Preparation**
   - Gather all critique files
   - Have the latest draft open
   - Create a new file for the revised version

2. **Revision Planning**
   Use this prompt to create a revision plan:
   ```
   Analyze this summary and critiques to create a structured revision plan.
   Determine the optimal order of critics and their focus areas based on the dependencies and priorities outlined.

   SUMMARY:
   [PASTE CRITIQUE SUMMARY]

   CRITIQUES:
   [PASTE ALL CRITIQUES]

   Please provide a structured plan for revisions:
   1. List major issues to address
   2. Order them by priority and dependency
   3. Identify specific sections needing work
   4. Note any potential conflicts between critiques
   ```

3. **Section Revision**
   For each section, use this prompt:
   ```
   Please revise this portion of text based on the following critique:

   CRITIQUE FOCUS: [SPECIFIC CRITIC'S FOCUS]
   [PASTE RELEVANT CRITIQUE]

   CURRENT TEXT:
   [PASTE SECTION]

   Requirements:
   1. Address the specific critique points
   2. Maintain narrative coherence
   3. Preserve strong elements
   4. Keep consistent style and voice
   5. Focus on [SPECIFIC AREA FROM CRITIQUE]

   Previous content (for context):
   [PASTE PREVIOUS SECTION END]

   Following content (for context):
   [PASTE NEXT SECTION START]
   ```

4. **Length Adjustment**
   If the draft needs length adjustment:
   ```
   Please [expand/condense] this text to approximately [TARGET] words while maintaining quality:

   [PASTE TEXT]

   Requirements:
   1. Focus on [adding essential details/removing redundancy]
   2. Maintain all key plot points
   3. Preserve character development
   4. Keep narrative flow smooth
   5. Ensure consistent pacing
   ```

5. **Final Polish**
   After addressing all critiques:
   ```
   Please polish this text for final revision:

   [PASTE REVISED DRAFT]

   Focus on:
   1. Smooth transitions between sections
   2. Consistent voice and style
   3. Clear character motivations
   4. Vivid sensory details
   5. Natural dialogue flow
   6. Proper pacing
   ```

## Best Practices

1. **Critique Analysis**
   - Read all critiques thoroughly
   - Note common themes
   - Identify contradictions
   - Prioritize structural issues

2. **Section Processing**
   - Work on one critique focus at a time
   - Check continuity between sections
   - Verify improvements address critiques
   - Maintain consistent style

3. **Quality Control**
   - Check word count frequently
   - Verify all critique points addressed
   - Review character consistency
   - Ensure plot coherence

4. **File Management**
   - Use descriptive draft names
   - Track critique implementation
   - Keep revision notes
   - Update index file

## Troubleshooting

1. **If Critiques Conflict**
   ```
   Please analyze these conflicting critique points and suggest a resolution:

   Critique A:
   [PASTE FIRST CRITIQUE]

   Critique B:
   [PASTE SECOND CRITIQUE]

   Requirements:
   1. Identify the core conflict
   2. Suggest a balanced approach
   3. Maintain story integrity
   4. Consider overall impact
   ```

2. **If Section Needs Refocus**
   ```
   Please refocus this section on its core purpose:

   INTENDED FOCUS:
   [DESCRIBE MAIN PURPOSE]

   CURRENT TEXT:
   [PASTE SECTION]

   Requirements:
   1. Strengthen core elements
   2. Remove distractions
   3. Maintain necessary context
   4. Improve clarity
   ```

3. **If Style Inconsistent**
   ```
   Please align this section's style with the story's voice:

   STYLE GUIDE:
   [PASTE STYLE NOTES]

   CURRENT TEXT:
   [PASTE SECTION]

   Requirements:
   1. Match narrative voice
   2. Adjust pacing
   3. Enhance tone
   4. Maintain authenticity
   ```

## Example Workflow

1. **Initial Setup**
   ```bash
   # Create revision file
   touch Chapter-1/drafts/draft-N-revised.md
   ```

2. **Critique Processing**
   - Analyze all critiques
   - Create revision plan
   - Order improvements
   - Note dependencies

3. **Section Revision**
   - Apply critiques in order
   - Check improvements
   - Maintain continuity
   - Verify word count

4. **Final Review**
   - Polish entire draft
   - Check all requirements
   - Verify improvements
   - Update files

## Notes

- Track changes systematically
- Save work frequently
- Check critique implementation
- Maintain consistent style
- Verify narrative flow
- Keep word count in range
- Document major changes

## Revision Checklist

- [ ] Read all critiques
- [ ] Create revision plan
- [ ] Process each section
- [ ] Check word count
- [ ] Verify improvements
- [ ] Polish final draft
- [ ] Update files
- [ ] Document changes 