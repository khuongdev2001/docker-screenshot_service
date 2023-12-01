# Introduction
Screenshot service is a simple tool written in node js, uses puppeteer api to help take screenshots, sharp to compress image size after capture, tool can run on docker


## Authors
- [@khuongdevcui](https://www.facebook.com/KhuongLaptop)


## API Reference

#### Screenshot website

```http
GET /screenshot
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `url` | `string` | **Required**. url website URL of the website you want to capture|
| `width` | `integer` |width of the photo after taking it **Default 800**|
| `height` | `integer` |height of the photo after taking it **Default 1000**|


## Usage

```docker
docker build -t screenshot_service .
```
```docker
docker run -dp 8080:80 screenshot_service
```
After Run localhost:8080
