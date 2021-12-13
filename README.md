## Bước 1

Tạo github repository và đẩy code react lên.

## Bước 2

Ở trong thư mục dự án của mình chạy lệnh `npm run build`, ta thấy một folder **build** được tạo ra: ![React folder structure](https://user-images.githubusercontent.com/87081336/145740027-31f33552-9e17-4d21-922e-9bf456797c81.png)

## Bước 3

Xoá dòng /build trong .gitignore:

![](https://user-images.githubusercontent.com/87081336/145740457-600998fa-0c4a-416e-a17b-59ea5147fa8b.png)

## Bước 4

Vào package.json và thêm "homepage": "./":

![package.json file](https://user-images.githubusercontent.com/87081336/145741710-9fe610b3-02e4-4048-bfeb-ca3d3ad45a79.png)

## Bước 5

Chạy lệnh: `git add build && git commit -m "Add build folder to deploy"`

## Bước 6

Push thư mục build lên nhánh gh-pages trên github:

`git subtree push --prefix build origin gh-pages`
