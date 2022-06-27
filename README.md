##  Train yolo neural networks on custom datasets
Yolo neural network model for custom training
    
    1 add the extra classes to yolo.cfg
    
    2 creates the annotations img1.png and img1.txt with the assigned boxes
     split data into the following folders:
     90% /data/images/training and 10% /data/images/validation/
    
    3 copies the annotations in the corresponding payments
     /data/lables/training/ and /data/lables/validation/
    
    3 re train (re trains yolo.weight) with train.py
    4 tests with new images
    
   
## Yolo format yolo.txt
`<object-class> <x> <y> <width> <height>`

`4 0.494545 0.521858 0.770909 0.551913`

- 4 is class_id
- 0.521858 is the y-axis value
- 0.770909 is the width of an object
- 0.551913 is the height of an object.


## Project folder structure

Main Folder

    --- data/
        --- dataset_name/
            --- images/
                --- img1.jpg
                --- img2.jpg
                ..........

            --- labels/
                --- img1.txt
                --- img2.txt
                ..........

            --- train.txt
            --- val.txt
