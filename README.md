# Tutorial-GagaNode

![IMG_20221224_215930_018](https://user-images.githubusercontent.com/109436048/209457370-99876dea-cd96-4f2f-a438-1a003f87e404.jpg)

## 1.Update package manager dan install curl, tar, dan ca-certificates:

### Ubuntu / Debian: 

sudo apt-get update -y && sudo apt-get -y install curl tar ca-certificates

### CentOS / Fedora: 

sudo yum update -y && sudo yum install -y curl tar ca-certificates


![IMG_20221225_121759_991](https://user-images.githubusercontent.com/109436048/209457405-b109a361-7851-4e81-b696-bc534c7f5883.jpg)

## 2.Download dan install aplikasi:

### Linux 64-bit: 

curl -o app-linux-amd64.tar.gz https://assets.coreservice.io/public/package/22/app/1.0.3/app-1_0_3.tar.gz tar -zxf app-linux-amd64.tar.gz rm -f app-linux-amd64.tar.gz cd ./app-linux-amd64 sudo ./app service 

### install Linux 32-bit: 

curl -o app-linux-386.tar.gz https://assets.coreservice.io/public/package/22/app/1.0.3/app-1_0_3.tar.gz tar -zxf app-linux-386.tar.gz rm -f app-linux-386.tar.gz cd ./app-linux-386 sudo ./app service install


![IMG_20221225_123349_351](https://user-images.githubusercontent.com/109436048/209457450-3cf431e7-506d-44c4-8d5a-8c3f1fc02312.jpg)

## 3.Mulai layanan aplikasi:

sudo ./app service start


![IMG_20221225_123612_752](https://user-images.githubusercontent.com/109436048/209457482-e57a3a38-13f8-4692-aaf4-0f2ed275c832.jpg)

## 4.Periksa status aplikasi:

./app status


![IMG_20221225_123728_152](https://user-images.githubusercontent.com/109436048/209457502-58baae5a-75c0-4af7-b3b6-8d635b664352.jpg)

## 5.Set token aplikasi: 

sudo ./apps/gaganode/gaganode config set --token=your token


![IMG_20221225_124009_233](https://user-images.githubusercontent.com/109436048/209457518-f3adb2e0-2f4d-48ce-912d-32434c918ac7.jpg)

## 6.Restart aplikasi:

./app restart


![IMG_20221225_124100_022](https://user-images.githubusercontent.com/109436048/209457530-ec6052db-739e-425d-9bee-b5325ae1b862.jpg)

## 7.Untuk referensi perintah lainnya, gunakan:

sudo ./app service install                    # install node
sudo ./app service start                      # start node
sudo ./app service stop                       # stop node
sudo ./app service remove                     # remove node
./app status                                  # check node running status
./app restart                                 # restart node
./app upgrade                                 # upgrade node
./app log                                     # check logs
./app -h                                      # check help


### Catatan: Tuliskan your token dengan token aplikasi yang Anda miliki. Jangan lupa untuk mengganti your token dengan token aplikasi yang sebenarnya.
