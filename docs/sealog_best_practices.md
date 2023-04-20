# Sealog Best Practices

## How to setup Event Templates in Sealog
It is important to remember that the primary way exported data is viewed is via spreadsheet.  "Event 
Values" and Event option names should be concise so to help with viewing.  Event option names 
should also be re-used across event templates where practical to minimize the total number of columns 
in the exported data.

Event option names can NOT be "id" or "comment". These are reserved keywords. 

## Event Option Types and their uses:
- **text**: when the value possibilities for the option are unknown and must be manually filled out 
when the event is submitted 
- **static text**: when the value is known and should not be altered
- **dropdown**: when the option is one of a long lists of possibilities
- **radio buttons**: when the option is one of a short list of possibilities
- **checkboxes**: when the option is one OR more of a list of possibilities

It is recommended to use the free_text input available to all event templates if an event should include a
description.

### Special Case: Samples
For sample events the “Event Value” should ALWAYS be “SAMPLE”
Sample templates MUST have the following event options:
 - Type: to specify the type of sample collected i.e. “biology, geology, eDNA, Niskin, etc”. This should be configured as a required option. If the desire is to have a dedicated button for a specific sample type then set this option as “static text” with the “value” set to the sample type i.e. “eDNA”.  If the event template is for multiple sample types then the “Type” option should have an option type of “dropdown” or “radio 
buttons”.
- Sample ID: to define the sample’s unique identification. This should be configured as a required option.
- Storage Location: the unique location on the vehicle where the sample is stored. This should be configured as a required option. This option should have an option type of "dropdown" or "radio buttons". Refer to the list of standard vehicle locations for how to populated the event option values. If the sample is collected with a sceince-supplied sampling apparatus (gas tights) then the option value should be a list of unique identifications for the apparatus type.  Ensure that the naming convention used for any sceince-supplied sampling apparatus does not conflict with the standard location names.
- Additional event options can be added to the sample event template so long as the option names do NOT include: “id”, “Type”, “Storage Location”, "Sample ID” or "comment"

### SOI Subastion’s standard naming convention for storage locations are:
- Bio-Box 1A (BB-1A)
- Bio-Box 1B (BB-1B)
- Bio-Box 2A (BB-2A)
- Bio-Box 2B (BB-2B)
- Bio-Box 3A (BB-3A)
- Bio-Box 3B (BB-3B)
- Bottle 01 (5L)
- Bottle 02 (5L)
- Bottle 03 (5L)
- Bottle 04 (5L)
- Bottle 05 (2.5L)
- Bottle 06 (2.5L)
- Quiver 01 (Q01)
- Quiver 02 (Q02)
- Quiver 03 (Q03)
- Quiver 04 (Q04)
- Quiver 05 (Q05)
- Quiver 06 (Q06)
- Quiver 07 (Q07)
- Quiver 08 (Q08)
- Quiver 09 (Q09)
- Quiver 10 (Q10)
- Quiver 11 (Q11)
- Quiver 12 (Q12)
- Quiver 13 (Q13)
- Quiver 14 (Q14)
- Quiver 15 (Q15)
- Quiver 16 (Q16)
- Suction 01
- Suction 02
- Suction 03
- Suction 04
- Suction 05
- Suction 06
- Suction 07
- Suction 08
