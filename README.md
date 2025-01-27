<h1>Implementation of remote DNS cache poisoning</h1>



<h2>Description</h2>
The goal of this project is for students to experience the remote DNS cache poisoning attack, commonly known as the Kaminsky DNS attack. The Domain Name System (DNS) functions as the Internet's directory service, converting domain names into IP addresses and vice versa. This process of DNS resolution typically occurs seamlessly in the background. However, DNS Pharming attacks can disrupt this resolution process, redirecting users to unintended, often malicious, destinations. This lab specifically examines the DNS Cache Poisoning attack, a particular method of DNS Pharming.
<br />


<h2>Languages and Utilities Used</h2>

- <b>C++</b> 
- <b>Visual Studio Code</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>
<section>
        <h3>RDMA Memory Registration</h3>
        <p>
            Memory registration is a prerequisite for RDMA operations, as RDMA devices require memory to be registered to ensure direct access. This involves:
        </p>
        <ul>
            <li>
                <strong>Pinning Memory:</strong> Allocating and locking physical memory pages to prevent them from being swapped out by the operating system.
            </li>
            <li>
                <strong>Generating Memory Keys:</strong> Associating registered memory regions with unique keys to facilitate access control during RDMA operations.
            </li>
            <li>
                <strong>Avoiding Re-registration Overheads:</strong> Efficient systems implement techniques such as memory pooling or caching registered memory regions to avoid repetitive registration costs.
            </li>
        </ul>
    </section>
    <section>
        <h3>Request Handling</h3>
        <p>
            Efficient request handling is crucial for leveraging RDMA's potential in real-time and large-scale data transfer. This includes:
        </p>
        <ul>
            <li>
                <strong>Work Queues (WQ):</strong> Managing RDMA operations through Send, Receive, and Completion Queues to process requests asynchronously.
            </li>
            <li>
                <strong>Zero-Copy Transfers:</strong> Utilizing RDMA's ability to directly read from or write to remote memory, eliminating the need for intermediate data copies.
            </li>
            <li>
                <strong>Flow Control and Synchronization:</strong> Coordinating RDMA requests to handle contention and ensure consistency between sender and receiver buffers.
            </li>
        </ul>
    </section>

