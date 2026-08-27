## Mission Overview 
Congratulations,  
Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by 
your supervisor. 
CloudNova Technologies has now assigned you to your first official project. 
Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern 
cloud computing. Your mission is to investigate the components of cloud infrastructure, identify how compute, 
storage, networking, and identity services work together, and document your findings as if you were preparing 
technical documentation for a client. 
Using the KillerCoda Playground, Linux tools, official cloud documentation, and your GitHub Cloud Computing 
Portfolio, you will complete a series of engineering tasks that simulate the planning phase of a cloud deployment. 

. 
## Mission Objectives 
At the end of this laboratory activity, you should be able to: 
 Explain the major components of cloud infrastructure.  
 Investigate the hardware and software resources available in a Linux environment.  
 Differentiate compute, storage, networking, and identity resources.  
 Interpret the relationship between cloud infrastructure components.  
 Create professional technical documentation using Markdown.  
 Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

| Component            | What was Found            |
| -------------------- | -------------------------------------------------- |
| Compute Resources    | Intel Xeon E312xx CPU, 1 CPU core, and 1.9 GiB RAM |
| Storage Resources    | 19G disk capacity and mounted file systems         |
| Networking Resources | IP addresses `172.30.1.2` and `172.17.0.1`         |
| Operating System     | Ubuntu 24.04.4 LTS                                 |

## Tools Used

| Tool                  | Purpose                                                    |
| --------------------- | ---------------------------------------------------------- |
| KillerCoda Playground | Used to access and investigate the Linux server            |
| Linux Terminal        | Used to execute commands and collect system information    |
| GitHub                | Used to store and document the laboratory work             |
| Markdown              | Used to format the technical documentation                 |
| Web Browser           | Used to access KillerCoda, GitHub, and cloud documentation |
| Draw.io (diagrams.net)| Used to create the cloud infrastructure diagram            |

## Linux Commands Executed

| Command                      | Purpose                                |
| ---------------------------- | -------------------------------------- |
| `cat /etc/os-release`        | Check the operating system information |
| `uname -r`                   | Check the kernel version               |
| `lscpu \| grep "Model name"` | Check the CPU model                    |
| `nproc`                      | Check the number of CPU cores          |
| `free -h`                    | Check the RAM and swap memory          |
| `df -h`                      | Check disk capacity and usage          |
| `findmnt`                    | Check mounted file systems             |
| `hostname`                   | Check the hostname                     |
| `hostname -I`                | Check the IP addresses                 |

## Skills Learned

I learned how to investigate a Linux server using basic command-line tools. I was able to identify the operating system, kernel version, CPU, CPU cores, RAM, disk capacity, mounted file systems, hostname, and IP addresses.

I also practiced organizing technical information using Markdown and managing my laboratory files in GitHub. The activity helped me understand the basic relationship between compute, storage, networking, and operating system resources in a cloud environment.

## Challenge Encountered

| Challenge                            | How I Handled It                                                                                                                         |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Understanding the `findmnt` output   | I reviewed the output carefully to understand the different mounted file systems.                                                        |
| Using the correct hostname command   | I initially used `hostname -l`, which was not the correct option for displaying the IP addresses. I corrected it by using `hostname -I`. |
| Organizing the technical information | I arranged the collected information into headings and tables to make the documentation easier to read.                                  |
| Formatting the README                | I practiced using Markdown headings, tables, code blocks, and lists in GitHub.                                                           |
