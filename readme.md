# Progit Summer internship 2019 interview

Programming exercise for the summer internship interview process

## 1. Problem description

A JPG picture is divided into equally sized tiles which make up a complete image.
Each tile has an `x` and `y` coordinate, `(x,y)`. The coordinate origin (0,0), starts from the upper left corner. `x` is the column position and `y` is the row position.

![alt text](https://i.imgur.com/5nvpHGv.jpg "Grid example")

_Example of a tile:_

![alt text](https://i.imgur.com/J00p08R.png "Tile example")

This tile has the coordinate of `(0, 1), x=0, y=1`

## 2. Progit Photo API

The `Progit photo API` returns a list of urls pointing to tiles of an image.
The files are named `{random-string}-x-y.jpg`, where `x` is the column position and `y` is the row position.

Example of a subset of the files in the response:

```
{
    "tiles": [
        "https://storage.googleapis.com/progit-interview-problem/images/plznkp-0-7.jpg",
        "https://storage.googleapis.com/progit-interview-problem/images/uvdjfb-7-4.jpg",
        "https://storage.googleapis.com/progit-interview-problem/images/nplkpg-12-6.jpg",
        "https://storage.googleapis.com/progit-interview-problem/images/elzsou-13-9.jpg",
        "https://storage.googleapis.com/progit-interview-problem/images/hplhbd-11-8.jpg",
        "https://storage.googleapis.com/progit-interview-problem/images/wupypj-11-4.jpg"
    ...]
}
```

**Ex:** The file `https://storage.googleapis.com/progit-interview-problem/images/plznkp-0-7.jpg` has the coordinates of `(0,7)`, `x=0, y=7`

Your solution show read the tile list from the API, download the image files associated with each tile and merge them in the correct order and finally save or print the merged picture.

## 3. Additional information / constraints

- All cells are the same in size
- The cell width and height is a natural number
- The width and height is not necessarily equal in size

## 4. Your solution should:

- Query the API and fetch the list of images
- Dynamically calculate the number of columns and rows. Try not to hardcode the col X row dimensions.
- Dynamically calculate the final size-dimension of the picture
- Print/show the image or save it to a .jpg file

You can use any programming language and libraries of choice. You do not need to solve the exercise completely, we are mainly interested in the way you approach the problem and how you choose to structure your code. If you run out of time before completing the problem you should still submit the solution! :)
