# ImageDiffOps

This Python wrapper can detect and extract the changed parts & coordinates of those parts from the images if any.

WOOOOAAAA----- "Coordinates" -Make use of coordinates to mask/fill or whatever you can think of doing in the image.


This Library can also be used to find a Similarity Score between two image

Steps to import and use:-

Download using pip command -- pip install ImageDiffOps

IMPORT:-

    from ImageDiffOps import ImageDiffOpsmageDiffOps
    import matplotlib.pyplot as plt


    imDfOps = ImageDiffOps("C:\\Users\\Desktop\\nik\\Test\\marked\\1.png","C:\\Users\\Desktop\\nik\\Test\\unmarked\\1.jpg")
    imgs,cord = imDfOps.detectDiffROI()
    imDfOps.SimilarityScore()

    imDfOps.SimilarityScore()
    import matplotlib.pyplot as plt


    plt.title("extracted image parts where change has happend")
    for img in imgs:
    
        plt.imshow(img, cmap=plt.cm.gray)
        plt.show()
