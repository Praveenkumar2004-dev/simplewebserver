# Developing a Simple Webserver

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

HTML content creation is done

### Step 2:

Design of webserver workflow

### Step 3:

Implementation using Python code

### Step 4:

Serving the HTML pages.

### Step 5:

Testing the webserver

## PROGRAM:
```
<!DOCTYPE html>
<html>
<head>
<title>Django</title>
</head>
<body>

<h1>Django</h1>
<p>This is Web Application Framework written in python</p>

</body>
</htmlclass myhandler(BaseHTTPRequestHandler):
     def do_GET(self):
         print("request received")
         self.send_response(200)
         self.send_header('content-type','text/html; charset=utf-8')
         self.end_headers()
         self.wfile.write(content.encode())
server_address = ('',8000)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running....")
httpd.serve_forever()  
```
## OUTPUT:
![simplewebserver](https://user-images.githubusercontent.com/119559827/214874689-4062147d-57e8-436e-bf91-98a21f2b8bed.png)

![webserver](https://user-images.githubusercontent.com/119559827/214874956-96549176-7e8f-4f53-af27-2a6cf4abceea.png)


## RESULT:
The program is executed succesfully
