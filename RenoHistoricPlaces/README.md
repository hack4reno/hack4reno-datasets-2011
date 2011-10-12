RenoHistoricPlaces.plist is an XML Property List. It contains a list of dictionaries that have the following keys: number, name, address, dateListed, note, latitude, longitude

On iOS 5, you can read in the file with the following code snippet:

NSURL *fileURL = [[NSBundle mainBundle] URLForResource:@"RenoHistoricPlaces" withExtension:@"plist"];
NSArray *artPieces = [NSArray arrayWithContentsOfURL:fileURL];

This will result in an array of dictionaries.
