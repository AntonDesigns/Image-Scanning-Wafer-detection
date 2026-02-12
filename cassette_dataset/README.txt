TRYMAX CASSETTE DATASET
======================

FOLDER NAMING CONVENTION:
Each folder name is the cassette configuration with 25 slot values separated by underscores.

SLOT VALUES (SlotOccupationState enum):
  1 = Empty (no wafer)
  3 = CorrectlyOccupied (wafer properly placed)
  4 = DoubleSlotted (two wafers in one slot)
  5 = CrossSlotted (wafer across slots)
  0 = Undefined (cannot determine)
  2 = NotEmpty (something there, unclear)

EXAMPLE:
  Folder: 1_3_3_3_3_4_3_3_3_3_3_3_3_3_3_3_3_3_3_3_3_3_3_3_3
  Means:  Slot 1 empty, Slots 2-5 correct, Slot 6 double-slotted, Slots 7-25 correct

HOW TO USE:
1. Set up the cassette in the configuration matching a folder name
2. Take multiple photos from the standard camera position
3. Save photos in the matching folder
4. Take photos at different angles/distances and note the metadata
5. If you encounter a new configuration, create a new folder with the correct name

PHOTOGRAPHY TIPS:
- Document camera distance (cm) for each session
- Note lighting conditions
- Take 10+ photos per configuration if possible
- Include some with people/objects in background (for robustness training)
- Vary slightly between photos (small angle changes)

ADDING NEW CONFIGURATIONS:
Just create a new folder with the correct 25-digit underscore-separated name.
The AI data loader will automatically pick it up.
