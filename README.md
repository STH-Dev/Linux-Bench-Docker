# Linux-Bench-Docker
Linux-Bench Docker version

This Docker image runs the Linux-Bench tests from Serve The Home (http://www.servethehome.com/)

Results are hosted at: http://beta.linux-bench.com/results/

To run:

Make sure Docker is installed:  
http://docs.docker.io/installation/#installation  

Quick instructions:
CentOS (requires EPEL)  
$ sudo yum install docker-io  

Ubuntu  
$ sudo apt-get update  
$ sudo apt-get install docker.io  
$ sudo ln -sf /usr/bin/docker.io /usr/local/bin/docker  


To run the benchmark, we pull the latest copy and then pass a directory to store results/logs, the default is current directory.  
<pre><code>
docker run -v `pwd`:/data linuxbench/linux-bench-docker
</code></pre>

