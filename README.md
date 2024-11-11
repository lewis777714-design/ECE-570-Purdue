# ECE-570-Purdue
Data downloading link:
https://www.cs.virginia.edu/~yq2h/jack/vision/voc.tar.gz

unzip the data within the same fold with the Project_code 

when training the model with LMT, Just change the known_labels
For example, I set the known label as 15. Typically known label equals 0.25 number of total label - 0.75 number of total label. 
known_labels=15
train_dataset = Voc07Dataset(img_dir=img_dir, anno_path=train_anno_path, image_transform=transform, labels_path=labels_path, known_labels=known_labels)
valid_dataset = Voc07Dataset(img_dir=img_dir, anno_path=valid_anno_path, image_transform=transform, labels_path=labels_path, known_labels=20)
