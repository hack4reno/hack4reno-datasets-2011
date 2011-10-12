PublicArtInventory.plist is an XML Property List. It contains a list of dictionaries that have the following keys: artistFirstName, artistLastName, year, type, artPiece, placement, location, street, city, state, budget, latitude, and longitude.

On iOS 5, you can read in the file with the following code snippet:

NSURL *fileURL = [[NSBundle mainBundle] URLForResource:@"PublicArtInventory" withExtension:@"plist"];
NSArray *artPieces = [NSArray arrayWithContentsOfURL:fileURL];

This will result in an array of dictionaries.
