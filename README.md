# Docker on Windows
This is the code repository for [Docker on Windows](https://www.packtpub.com/virtualization-and-cloud/docker-windows?utm_source=github&utm_medium=repository&utm_campaign=9781785281655), published by [Packt](https://www.packtpub.com/?utm_source=github). It contains all the supporting project files necessary to work through the book from start to finish.

## About the Book
Docker is a platform for running server applications in lightweight units called containers. You can run Docker on Windows Server 2016 and Windows 10, and run your existing apps in containers to get significant improvements in efficiency, security, and portability.

This book teaches you all you need to know about Docker on Windows, from 101 to deploying highly-available workloads in production. This book takes you on a Docker journey, starting with the key concepts and simple examples of how to run .NET Framework and .NET Core apps in Windows Docker containers. Then it moves on to more complex examples—using Docker to modernize the architecture and development of traditional ASP.NET and SQL Server apps.

The examples show you how to break up monoliths into distributed apps and deploy them to a clustered environment in the cloud, using the exact same artifacts you use to run them locally. To help you move confidently to production, it then explains Docker security, and the management and support options.

The book finishes with guidance on getting started with Docker in your own projects, together with some real-world case studies for Docker implementations, from small-scale on-premises apps to very large-scale apps running on Azure.

## Instructions and Navigation
All of the code is organized into folders. For example, Chapter02.



The code will look like the following:
```
# registry image
FROM microsoft/nanoserver:10.0.14393.1358
SHELL ["powershell", "-Command", "$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]

ENV DATA_PATH="C:\data" `
    REGISTRY_STORAGE_FILESYSTEM_ROOTDIRECTORY="G:\\"

RUN Set-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\Session Manager\DOS Devices' -Name 'G:' -Value "\??\$($env:DATA_PATH)" -Type String

```



## Related Products
* [Build Your Own PaaS with Docker](https://www.packtpub.com/virtualization-and-cloud/build-your-own-paas-docker?utm_source=github&utm_medium=repository&utm_campaign=9781784393946)

* [Docker Networking Cookbook](https://www.packtpub.com/networking-and-servers/docker-networking-cookbook?utm_source=github&utm_medium=repository&utm_campaign=9781786461148)

* [Docker: Creating Structured Containers](https://www.packtpub.com/virtualization-and-cloud/docker-creating-structured-containers?utm_source=github&utm_medium=repository&utm_campaign=9781786465931)
### Download a free PDF

 <i>If you have already purchased a print or Kindle version of this book, you can get a DRM-free PDF version at no cost.<br>Simply click on the link to claim your free PDF.</i>
<p align="center"> <a href="https://packt.link/free-ebook/9781785281655">https://packt.link/free-ebook/9781785281655 </a> </p>