# Introduction to Docker

Docker is really just Linux containers which are a type of virtualization.

Virtualization has its roots at the beginning of computer science when large, expensive mainframe computers were the norm. How could multiple programmers use the same single machine? The answer was virtualization and specifically virtual machines which are complete copies of a computer system from the operating system on up.

If you rent space on a cloud provider like AWS they are typically not providing you with a dedicated piece of hardware. Instead you are probably sharing a physical server with hundreds or even thousands of other clients.

What’s the downside to a virtual machine? Size and speed. A typical guest operating system can easily take up 700MB of size. So if one physical server supports three virtual machines, that’s at least 2.1GB of disk space taken up along with separate needs for CPU and memory resources.

Most computers rely on the same Linux operating system, so what if we virtualized from that level up instead? Wouldn’t that provide a lightweight, faster way to duplicate much of the same functionality?

The answer is yes. And in recent years Linux containers, also known as “containerization,” has become increasingly popular. For most applications, a virtual machine provides far more resources than are needed and a container is more than sufficient.

This, fundamentally, is what Docker is. A way to implement Linux containers!
## Important Facts About Docker

* Dockerfile is a list of instructions for creating an image
* Images are made up of one or more layers
* Containers are a running instance of an image
* docker-compose.yml controls how to run the container
* Containers are stateless and ephemeral in nature. We can link
* the local filesystem via volumes but things become more complex with databases (which we didn’t cover here).
