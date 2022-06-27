yolo  TRAINING CUSTOMIZZATO
    
    1 aggiungi le classi in piu su yolo.cfg 
    2 crea le annotazioni img1.png e img1.txt con i box assegnati
    	dividi dati nelle seguenti cartelle:
    	 90% /data/images/training e 10% /dataimages/validation
    
    3 copia le annotazioni nei corrispettivi
    	     /data/lables/training/ e /data/lables/validation/
    
    3 re train (ri allena yolo.weight) with train.py
    4 test con nuove immagini
    
   
## Yolo format yolo.txt
`<object-class> <x> <y> <width> <height>`

`4 0.494545 0.521858 0.770909 0.551913`

4 is class_id
0.521858 is the y-axis value
0.770909 is the width of an object
0.551913 is the height of an object.


## Project folder structure
Main Folder
--- data
    --- dataset name
        --- images
            --- img1.jpg
            --- img2.jpg
            ..........
        --- labels
            --- img1.txt
            --- img2.txt
            ..........
        --- train.txt
        --- val.txt
