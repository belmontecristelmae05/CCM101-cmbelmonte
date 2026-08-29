## Mission Overview 
Congratulations,  
Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by 
your supervisor. CloudNova Technologies has now assigned you to your first official project. Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern cloud computing. Your mission is to investigate the components of cloud infrastructure, identify how compute, 
storage, networking, and identity services work together, and document your findings as if you were preparing technical documentation for a client. Using the KillerCoda Playground, Linux tools, official cloud documentation, and your GitHub Cloud Computing Portfolio, you will complete a series of engineering tasks that simulate the planning phase of a cloud deployment. Remember: Great cloud engineers build systems—but exceptional cloud engineers document and justify 
every design decision. 

## Mission Objectives 
At the end of this laboratory activity, you should be able to: 
 Explain the major components of cloud infrastructure.  
 Investigate the hardware and software resources available in a Linux environment.  
 Differentiate compute, storage, networking, and identity resources.  
 Interpret the relationship between cloud infrastructure components.  
 Create professional technical documentation using Markdown.  
 Continue building a structured GitHub Cloud Computing Portfolio.  

# Cloud Infrastructure Components

| Component            | What Was Found                                     |
| -------------------- | -------------------------------------------------- |
| Compute Resources    | Intel Xeon E312xx CPU, 1 CPU core, and 1.9 GiB RAM |
| Storage Resources    | 19G disk capacity with mounted file systems        |
| Networking Resources | `172.30.1.2` and `172.17.0.1`                      |
| Operating System     | Ubuntu 24.04.4 LTS                                 |

# Tools Used

| Tool                   |
| ---------------------- | 
| KillerCoda Playground  | 
| Linux Terminal         |
| GitHub                 |
| Markdown               |
| Web Browser            |
| Draw.io (diagrams.net) |

# Linux Commands Executed

| Command                      |
| ---------------------------- | 
| `cat /etc/os-release`        |
| `uname -r`                   |
| `lscpu \| grep "Model name"` |
| `nproc`                      |
| `free -h`                    |
| `df -h`                      |
| `findmnt`                    |
| `hostname`                   |
| `hostname -I`                |

# Skills Learned

I learned how to inspect a Linux server and collect useful system information through terminal commands. I became more familiar with checking the CPU, memory, disk, operating system, file systems, hostname, and network addresses.

I also improved my ability to organize technical information using Markdown tables and headings. Managing the laboratory outputs through GitHub gave me additional experience in keeping technical work properly documented.

# Challenges Encountered

| Challenge                                | How I Handled It                                                                  |
| ---------------------------------------- | --------------------------------------------------------------------------------- |
| Understanding some Linux command outputs | I reviewed the results and identified what information each command provided.     |
| Reading the `findmnt` output             | I examined the mounted locations and file system types carefully.                 |
| Getting the correct IP address           | I used `hostname -I` to display the server's IP addresses.                        |
| Organizing the collected information     | I grouped the results based on their corresponding infrastructure components.     |
| Preparing the GitHub documentation       | I used Markdown tables and headings to make the information easier to understand. |

