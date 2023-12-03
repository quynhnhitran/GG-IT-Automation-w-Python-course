# 1. Module 1
## 1.1 Distributed systems (Hệ thống phân tán)
- is a collection of software components that are designed to work together even though they’re on separate servers.
- là một tập hợp các thành phần phần mềm được thiết kế để làm việc cùng nhau, ngay cả khi chúng đặt trên các máy chủ riêng biệt.

- A common example of a distributed system woulb be a website that contains:
  + Presentation logic
  + Business logic
  + Database engine
  + Web server

- Applications: are used in various applications, including cloud computing, web services, peer-to-peer networks, content delivery networks (CDNs), grid computing, and more.

- <i> Key takeaways: </i>
  + Definition: collaborate across separate servers, shared network.
 

## 1.2 NALSD
- Definition:
  + Non-abstract large system design
  + give SREs (site reliability engineers) the ability to access, design, and evaluate large systems.

- Two phrases:
  + Phase 1:
      * continuous refinement through feedback, prototyping, and feasibility studies.
      * Qúa trình lặp lại và liên tục hoàn thiện
  + Phase 2:
      * evaluates the system's feasibility and resilence at scale, considering how it will perform under significant load increases.

## 1.3 Built-In Libraries vs. External Libraries
  -  PyPI -- also known as the Python Package Index (https://pypi.org)
  -  In this module, we’re going to be transforming and converting images. To do that, we'll be using a popular library for image manipulation: the Python Imaging Library (PIL). The original PIL library hasn't been updated since 2009 and does not support Python 3. Fortunately, there's a current fork of PIL called Pillow, that properly supports Python 3 and is kept up-to-date. The Pillow library is packaged with the name pillow, but the module name in Python is still PIL.
>  ``` $ pip3 install pillow ```

## 1.4 Application Programming Interfaces (APIs) 

## 1.5 Generate and manage containers
### 1. Generating image containers
- To build a container image, you create a Dockerfile, which contains step-by-step instructions for Docker to package your application along with all its dependencies.
- Link reference: https://docs.docker.com/get-started/02_our_app/
- Install:
    + Docker Desktop
    + Git client
    + VS Code (IDE or a text editor to edit files)
- Get the app:
    + ``` git clone https://github.com/docker/getting-started-app.git ```
    + ![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/0ab6786a-1178-413b-b5ca-13f06acbd285)
- Build the app's image
    + Tạo 1 Dockerfile (cùng cấp với package.json)
        * Tạo trên vs code sau khi clone git về
        * Dùng WCP để run lệnh:
          ``` cd \path\to\getting-started-app ``` (cd tới thư mục)
          ``` type nul > Dockerfile ``` (create an empty file)
     + Add content sau vào file Docker:
          ``` # syntax=docker/dockerfile:1
              FROM node:18-alpine
              WORKDIR /app
              COPY . .
              RUN yarn install --production
              CMD ["node", "src/index.js"]
              EXPOSE 3000 ```
    + Build the image
        ``` cd /path/to/getting-started-app ```
        ``` docker build -t getting-started . ```
- Start an app container
    + Run your container using docker run command: ``` docker run -dp 127.0.0.1:3000:3000 getting-started ```
    + open your web browser to http://localhost:3000: ![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/a0621ace-9e2a-4120-ba66-e30fcc480e95)

- Take a look: see one container running:
  + Docker Desktop's graphical interface ![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/0423c60c-77df-480a-bc1b-5ace859016c7)
  + CLI: ![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/b5c83f87-3c99-411b-bc73-90acaa10eef3)
 
### 2. Choose a base image
- Here are some of the most popular base images:
  + Debian  and Ubuntu: containers that boot into a full-featured, general Linux environment 
  + Alpine Linux: a stripped-down image designed to result in small, fast containers
  + Python: great for running Python apps
 
### 3. Create a Dockerfile

### 4. Build a Docker image

![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/a8f57597-1c61-4ecf-82ee-3895fea9e226)

![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/5cbf03b3-abdf-4432-868d-b7a60b38b1a3)

## 1.6 Build a container using VS Code and Docker
- DevContainer option:
  + Microsoft supports  a new open-source standard called DevContainer that extends the use of Docker in the development cycle. Rather than build your container every time you want to test it, with DevContainer, you can actually develop and debug your code inside a container.
  + DevContainer is also compatible with GitHub Codespaces, which means you can run your IDE in the cloud. Instead of spending time setting up your local development environment just right, you can add a devcontainer.json file to your Git repository and develop in the cloud with a development environment that is fully version controlled.
  + You can read more about DevContainer here: https://code.visualstudio.com/docs/devcontainers/containers
  +  ![image](https://github.com/quynhnhitran/GG-IT-Automation-w-Python-course/assets/128997325/6b91d0ca-de33-42d8-aeb7-2022c29d7af1)
- Key takeaways
> VS Code's integration with Docker simplifies the process of container creation, orchestration, and management, enabling developers to build, test, and deploy applications more efficiently. Containers offer a consistent and isolated environment for development, eliminating the “it works on my machine” problem and ensuring seamless collaboration across teams.

# How to Use PIL for Working With Images
- Python Imaging Library
- resize an image and save the new image with a new name:
  ``` from PIL import Image
im = Image.open("example.jpg")
new_im = im.resize((640,480))
new_im.save("example_resized.jpg") ```

-  rotate an image:
  ``` from PIL import Image
im = Image.open("example.jpg")
new_im = im.rotate(90)
new_im.save("example_rotated.jpg") ```

- combine these operations into just one line that rotates, resizes, and saves:
  ``` from PIL import Image
im = Image.open("example.jpg")
im.rotate(180).resize((640,480)).save("flipped_and_resized.jpg") ```
