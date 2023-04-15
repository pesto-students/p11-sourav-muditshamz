# Assignment Solutions

### What is a protocol stack, and how is it used in web development?
Protocol stacks are a layered collection of protocols that work together to provide communication services. Each protocol in the stack is responsible for a specific task, and by layering them, we can create a more robust and reliable system.
These layers are divided in such a way that each layer uses the output of the layer right below it, performs the allocated functions, and prepares the input for the next layer, or vice versa. This layered architecture is called the five-layer internet protocol stack.
![5 layers to Protocol stack](https://www.educative.io/answers/what-is-the-five-layer-internet-protocol-stack#:~:text=Application%20Layer-,Transport,-Layer )
##### Physical layer
The physical layer is responsible for breaking the data frame into bits, converting it into a form that can be transmitted over the physical communication line, and transferring it. This form could be light pulses (fiber-optic), radio waves for wireless communication, or electric pulses (for wired communication).On the receiving end, the physical layer collects the stream of bits and reassembles it into a data frame that is then passed onto the link layer for further processing.
The protocols and rules used at this layer are dependent on the kind of communication medium being used. For example, ethernet (link layer protocol) has different physical layer protocols for twisted-pair cable, coaxial cable, and fiber optic cable.

##### Link layer
When a packet is being transferred over the internet, several intermediate devices are between the two end systems. These devices may be routers, switches, or other computers. The link layer is responsible for communication between one device and its immediate neighbor.
The protocols and methods used for one link might differ from the protocol used in the next immediate link, even if the destination and data packet remain the same.The link layer adds a header with its information on top of the packet it receives from the network layer. The data packet at the link layer is called a frame.The link-layer is mostly implemented in the network adapter/network interface card (NIC), and technologies like ethernet, Wi-Fi, token ring, etc., are associated with the link layer.

##### Network layer
The network layer is responsible for transferring data from one system to another on the network. The transport layer passes a segment and the destination address to the network layer. Then, it is the responsibility of the network layer to transfer the data to the destination end-system over the network. This layer also takes care of the routing of data on intermediate routers.
The network layer adds a header and a trailer with its information on top of the packet received by the transport layer. The data packet at the network layer is called a datagram.
The main protocol used at the network layer to transfer data is Internet Protocol (IP). This protocol makes use of IP addresses to identify each system connected to the internet. The two versions of IP protocol are as follows:
IPv4: widely used protocol for communication over the internet and uses a 32-bit IP address
IPv6: proposed to replace IPv4 with the IP addresses of 128-bits because 32-bit IP addresses will be insufficient with the high number of computers being connected to the internet
Another protocol used at this layer for error-reporting is the Internet Control Message Protocol (ICMP). ICMP requests the sender to resend the data if the data is not received or received in the wrong order on the other end. It is simply a protocol that transfers information about the data, not the data itself. It is different from IPv4 or IPv6 as it does not rely on TCP or UDP. It does not ensure a reliable connection before sending a message.

##### Transport layer
On the sending end, the transport layer is responsible for collecting the application layer message from the relevant end-point and transferring it to the network layer to be communicated over the network. The receiving end collects the message from the network layer and passes it on to the relevant end-point where the application layer can access that message.
These end-points are called sockets. The transport layer uses a unique identifier called a port number to identify the correct socket or application.
The message received from the application layer might be broken into chunks at this layer.
The transport layers add a header with its own information on top of the message received from the application layer. The unit of data at the transport layer is called a segment.
The two important protocols used in the transport layer are:
Transmission Control Protocol (TCP): for reliable and connection-oriented data transfer
User Datagram Protocol (UDP): for fast, unreliable, and connection-less data transfer
Connection-oriented means that TCP establishes the connection first and then transmits the data. On the other hand, UDP is connection-less, which means that it just sends the data without checking if it is being received or not.

##### Application layer
As suggested by its name, the application layer is responsible for communication between applications running on two different end systems. A message or data transferred from one end is readable for the corresponding application on the other end. These applications include web browsers, email clients, etc.
At the application layer, the data being transferred is called a message.
The protocols used at the application layer include:
Hypertext Transfer Protocol (HTTP): for transferring HTML web documents
File Transfer Protocol (FTP): for transferring files
Simple Mail Transfer Protocol (SMTP): for transferring e-mail messages
Domain Name System (DNS): for translation of human-friendly domain names into IP addresses


### What are the different types of web servers, and how do they differ in terms of functionality and performance?
1. Web server
An open-source web server is used for accessing the world wide web through public domain software. These servers connect stored information from an internet website to your own computer. Web servers store information for the internet that is retrieved via "HTTP" code and sent to your web browser. This is one of the most widely used types of servers.
2. Proxy server
Proxy servers act as a bridge between a host server and a client server. A proxy sends data from a website to your computer IP address after it passes through the proxy's server. This practice adds a layer of security since the information is requested then transferred from the source to the proxy server and never directly from a client to another user. A proxy server can filter out various harmful internet entities.
3. Virtual machine (VM)
As their name suggests, virtual machines store and connect data strictly through virtual space. To create a virtual machine, IT teams use a hypervisor, also known as a virtual machine monitor (VMM), which is software that can run thousands of virtual machines through only one piece of physical hardware. This method of server virtualization is widely used for data transfer and storage because they are the most cost-effective type of server to run.
4. File transfer protocol (FTP) server
FTP servers are used to relocate files from one computer to another. Uploaded files move from your computer to the server while downloaded files are extracted from the server onto your device. File transfer protocol also refers to the method of using a server to connect one computer to another in order to share data safely.
5. Application server
These servers connect clients to software applications through virtual server connections. This allows users to bypass downloading data to their own hardware in order to access applications. Application servers can effectively host large amounts of application data to many users at once, making them ideal for businesses.
6. File server
A file server stores data files for multiple users. They allow for faster data retrieval and saving or writing files to a computer. This is a basic type of server used commonly by organizations where lots of users need access to files that are more conveniently and safely stored on a server than a personal computer.
7. Database server
Database servers function as large storage spaces that organizations use and access to run multiple programs to meet their needs. A database server can run independently of any database architecture.
8. Mail server
A mail server stores and delivers mail for clients through email service platforms. Because mail servers are set up to continually connect to a network, individual users can access their email without running any systems through their own devices.
9. Print server
A print server connects remotely to local computers to print through a network. These servers give businesses the ability to use a single printer to serve an entire department. Some printers even come with their own built-in server ready to join a network once they're installed in an office area.
10. Domain name system (DNS) server
These servers transform readable computer domain names into computer language IP addresses. The DNS server takes search data from a user and finds the requested address to deliver to the client device.
11. Collaboration server
When work needs to be shared across multiple users, a collaboration server makes it easy to connect. These servers allow you to share and store files, applications and other large amounts of data.
12. Gaming server
Large gaming networks use servers to connect users from around the world. These servers host multi-player online games.
13. Monitoring and management server
Monitoring and management servers function in several capacities. First, they record and track digital transactions and receive user requests. Others simply monitor and don't actively participate in user operations. Monitoring servers are responsive to network administrators who survey network health to check for threats or bugs in the system.

### What is web hosting, and what are the different types of hosting services available for websites?
- Shared Hosting
Shared hosting implies that you need to share the server with others, which means your website is hosted on a server shared by other sites. If it provides you all the tools and resources required to create and manage your website. Shared hosting is highly affordable; hence to minimize costs, most people start an online business with a Shared hosting plan. This hosting type is specially made for users managing a single website that is not most likely to get a ton of traffic initially. But in case the traffic on your site increases, you will need to switch to another hosting service as the shared server won’t be able to handle the load and will also affect the performance of the other websites on the same server.

- Who should opt for it:
If you want to host a website that runs like a personal blog or is a new business just starting out, then shared hosting is a good option until your website starts getting a constant stream of steady traffic.
Likewise, shared hosting also works if your website is under a development phase, and you need a base to test it.
As shared hosting is cheaper, so it’s best suitable for any person who is on a shoestring budget.
Small to medium enterprises with low traffic can use shared hosting if at an affordable cost if they do not have a high demand for resources to expand their business and client base on a global level.
- Dedicated Hosting
Having a dedicated hosting server means renting out one physical server from a hosting company. With dedicated servers, the clients get full control (termed as “root” permissions in Linux), which allows them to configure it to meet their own unique needs. With a dedicated server, you don’t have to worry about other people’s sites hogging up your resources and slowing your website down, unlike a shared hosting server. Generally, the highest level of server you would need for a growing business with a lot of website traffic is a dedicated hosting server. While the costs of it are significantly higher than shared and VPS hosting, the pricing is influenced by the number of resources; you need, such as RAM, bandwidth, storage space, amongst other things. Hence your business shall be at a point where it can easily afford the necessary costs of having a dedicated server.

- Who should opt for it:
Use a dedicated server if you’re expecting a massive amount of traffic into your website.
While a dedicated server is better than the traditional VPS server, it still lacks in its scalability. But a dedicated server will be extremely necessary if your website has specialized hardware requirements.
The dedicated server will also be necessary if you want to meet the high customization needs of your business.
The dedicated server is unbeatable from a security point of view, so if your business demands a massive amount of control over data privacy, then it is recommended to use a dedicated server since it keeps you are separate from everyone else.
- Virtual Private Server (VPS) Hosting
Virtual private servers act like multiple separate servers but share one physical server. A VPS hosting server is a stepping stone between getting your dedicated machine and shared hosting. A VPS server avoids the cost of a dedicated server while also preventing the problem of having your hosting neighbors slow down your website. Virtual Private Server hosting is the next step up from shared hosting because even though each VPS instance shares hardware resources, it allocates a dedicated slice of the computing resources. VPS hosting is a popular option for website owners looking for an upgrade from traditional shared hosting because it offers a balance of all points, including services and cost.

- Who should opt for it:
Some low-end VPS packages are not too expensive when compared to shared hosting, so it is suitable for businesses on a limited budget.
If you need a limited number of resources to be allocated to your website, with limited space and computing power, VPS hosting will likely keep your site running smoothly.
VPS hosting is ideal for growing websites even on the other end of the scale; for example, choosing a high-end VPS plan will be a better choice than a low-end dedicated server.
If you have a budget that allows you to spend $13 or more per month on hosting, then it is advised for you to choose a VPS-based plan over traditional shared hosting.
- Managed WordPress Hosting
Managed WordPress hosting is a type of hosting package that is more of a combination of hosting types with additional services. In essence, it is not a typical hosting type, but the WordPress platform has become so widely used that it’s worth mentioning. Managed WordPress hosting is especially for those who aren’t all that technically proficient but want to manage and run their WordPress site smoothly. It is a service where the hosting company operates all the techy stuff related to keeping your WordPress site up. This includes handling things such as updates, speed improvement, scalability, security, and daily backups. The idea is to allow you to focus on your business, rather than tinkering with WordPress every other hour. While it is not as inexpensive as shared web hosting, it is an excellent option for both established businesses and start-up businesses that use the WordPress platform.

- Who should opt for it:
Managed WordPress hosting is suitable for you if you are running a small personal blog website though you can also opt for free hosting or a small Shared hosting plan.
Especially if you own a small business or are a freelancer and your website gets quite a bit of traffic, then Managed WordPress hosting is an excellent option for you.
This hosting type is beneficial for people who aren’t technically savvy or simply would not wanna fiddle with the behind-the-scenes stuff.
With Managed WordPress hosting, you don’t have to worry about updates or deal with security issues, uptime issues, and speed problems.
It is ideal for you if you’re looking for a hassle-free experience limited flexibility of resources but great support.
- Reseller Hosting
Reseller hosting makes it is possible for you to start your own hosting business and generate clients under your brand. In Reseller hosting, you employ the services of another parent web hosting company and utilize their resources to sell it as your own. It is an option that involves one hosting provider company that rents bandwidth and hard drive space, another mid-size business company, which then rents the space to third parties entrepreneurs and small businesses. In reseller hosting, you get a shared environment where you create multiple shared accounts under one master account.

- Who should opt for it:
If you are looking for scalable web hosting that goes beyond traditional hosting services, then reseller hosting is an excellent option for you.
If you are planning to set up your own web hosting brand, then reseller hosting is the best to get started
It eliminates the high investment cost for a start-up web hosting business as well as manages the task of server maintenance.
Additionally, development firms, web designers, or any individual or company that needs to host multiple website accounts can choose reseller hosting.

### What is scaling, and why is it important for web applications? How does scaling differ for vertical and horizontal scaling?
The scalability of an application can be measured by the number of requests it can effectively support simultaneously. The point at which an application can no longer handle additional requests effectively is the limit of its scalability. This limit is reached when a critical hardware resource runs out, requiring different or more machines. Scaling these resources can include any combination of adjustments to CPU and physical memory (different or more machines), hard disk (bigger hard drives, less “live” data, solid state drives), and/or the network bandwidth (multiple network interface controllers, bigger NICs, fiber, etc.).
- Horizontal Scaling
 (scaling out)
1. In a database world, horizontal scaling is usually based on the partitioning of data (each node only contains part of the data).
2. Downtime, In theory, adding more machines to the existing pool means you are not limited to the capacity of a single unit, making it possible to scale with less downtime.
3. Concurrency, Also described as distributed programming, as it involves distributing jobs across machines over the network. Several patterns associated with this model: Master/Worker*, Tuple Spaces, Blackboard, MapReduce.
4. Message passing,In distributed computing, the lack of a shared address space makes data sharing more complex. It also makes the process of sharing, passing or updating data more costly since you have to pass copies of the data.

- Vertical Scaling
 (scaling up)
1. In vertical scaling, the data lives on a single node and scaling is done through multi-core, e.g. spreading the load between the CPU and RAM resources of the machine.
2. Downtime, Vertical scaling is limited to the capacity of one machine, scaling beyond that capacity can involve downtime and has an upper hard limit, i.e. the scale of the hardware on which you are currently running.
3. Concurrency, Actor model: concurrent programming on multi-core machines is often performed via multi-threading and in-process message passing.
4. Message passing,In a multi-threaded scenario, you can assume the existence of a shared address space, so data sharing and message passing can be done by passing a reference.

### What is SEO (Search Engine Optimization), and how can web developers optimize their websites for better search engine rankings?
Search engine optimization (SEO) is the art and science of getting pages to rank higher in search engines such as Google. Because search is one of the main ways in which people discover content online, ranking higher in search engines can lead to an increase in traffic to a website.

1. Use Keywords Throughout Your Content
Using SEO-friendly keywords is critical to improving your website’s position on search engine result pages (SERPs).
When writing content, incorporate relevant keywords to help search engines recognize what your website is about. You can get them by conducting keyword research.
Search your main keyword on the search engine, and you will find other related terms in the results. For example, if you search for pet toys, you will see other keywords, such as dog toys and pet supplies.
Additionally, consider using tools like Google Trends or Ahrefs to better understand popular topics and your audience’s search intent.
Google Trends is useful for comparing two different terms and seeing how often people search for them over time.
On the other hand, Ahrefs can show you more advanced metrics like keyword volume and traffic potential. These factors help you choose target keywords to use in your content.
Once you find your targeted keywords, try to apply them naturally and strategically. Avoid including keywords in content without considering their context and readability. This can negatively impact user experience and reduce your chance of appearing on the top of the SERPs.

2. Use Header Tags
Another way to create an SEO friendly website is by utilizing header tags properly. They are HTML elements that give structure and meaning to a web page’s content, helping search engines understand its contents.
Header tags consist of <h1> to <h6> HTML elements. Focus on your <h1> and <h2> tags since they are commonly used for the content’s title and headings. List your keywords and include them in these tags accordingly.
Try to also include relevant SEO keywords to other headers once you optimize all the <h1> tags. Apply this method consistently whenever you publish content to improve your SEO rankings.
As a result, search engine crawlers will know that this page contains content related to those terms and be able to accurately index your site for relevant content. This will improve your page ranking on the SERPs, enabling you to reach the right audience.

3. Have a Clean URL Structure
A clean URL structure is essential to creating an SEO-friendly website. An SEO-friendly URL should be easy to read, simple to understand, and related to the page’s context.
Search engines use URLs to crawl and index websites, so having SEO-friendly URLs helps them understand what content is on each page. Do this by including the target keyword on the URL.
For example, a URL for a page about an SEO-friendly website design could look like this: www.examplewebsite.com/seo-web-design.
Avoid using long query strings with numbers, like /top-23-seo-web-design-practises-in-2023-for-top-professionals – this can make them hard to read and less SEO-friendly.
With SEO-friendly URLs, search engines can crawl your website more efficiently and accurately, increasing your site’s position in relevant search results.

4. Include Keyword-Rich Anchor Text in Your Links
Anchor texts are clickable words that take users to another page or section of the website when clicked. Adding SEO-friendly anchor texts allows search engines to understand the content better and rank it higher.
When creating an SEO-friendly anchor text, you should focus on the keywords that relate to your website.
Think of words or phrases relevant to the content and best explain what it links to. For example, if you’re linking to a page about SEO tips, use anchor text such as Learn SEO tips or SEO strategies.
Remember, SEO-friendly anchor texts should be relevant to the linked page and give search engines an idea of what the content is about. It’s also important to avoid keyword stuffing in your anchor text, as this could negatively impact the website’s SEO score.

5. Make Sure the Website Is Mobile-Friendly
Making an SEO-friendly website involves more than optimizing the content – it also includes building a mobile-friendly website.
In fact, mobile users contributed nearly 59% of the global website traffic in the second quarter of 2022. As a result, Google and other search engines consider a website’s mobile-friendliness as an important factor in ranking search results.
Because of that, your website should be able to load quickly on mobile devices. Ensure your website’s design is responsive, which means it can adjust to different screen sizes.
Fortunately, most ready-to-use themes for WordPress or other website platforms come with a mobile version.
Don’t forget to use tools like Google’s Mobile-Friendly Test to check if your site is up to the current standards.

6. Optimize Images
Optimizing images for SEO is a great way to improve the visibility of your website in search engines. You can take several steps to ensure that your images are SEO-friendly and help boost your SEO performance.
Make sure that you give each image an appropriate file name. It should include keywords related to the content of the image. This will help search engines identify the image’s content, which can lead to better visibility on the SERPs.
Reduce the size of your images before you upload them to your website. Larger file sizes can slow your page down, negatively affecting SEO performance.
Consider compressing your images to reduce their size while maintaining their quality. WordPress users can use tools like Smush and EWWW Image Optimizer to optimize image size for their websites.
Additionally, don’t forget to add alternative text for each image. Alt text is a piece of HTML code that describes the image’s content and will appear if an image fails to load properly.
Adding this information helps search engines recognize the context within images, improving your SEO performance.
Finally, consider adding short captions under your images. Doing so can also give more context to the images, which improves user experience.

7. Make Sure Your Web Pages Load Fast
Search engines prioritize websites that load quickly and can provide an optimal user experience. A slow website will hurt your SEO effort, reduce customer satisfaction, and make it harder for search engines to crawl your content.
Fortunately, there are several steps you can take to optimize your website, including:
Reduce server response time by optimizing HTTP requests.
Compress images and other media files, reducing their size while maintaining quality.
Leverage browser caching to store frequently accessed files locally in each user’s browser instead of downloading them every time.
Use a content delivery network (CDN) to distribute the load of hosting images, videos, and other static content across multiple servers worldwide.
Get a better web hosting plan with higher bandwidth.
Consider using tools like Google’s PageSpeed Insights to check if your site meets the standard and get various insights on how you can improve its loading speed.

8. Use Social Media to Promote Your Content
Promoting your content on social media is one of the best ways to create an SEO-friendly website. Your content can reach a wider audience, resulting in more backlinks that search engines will index and consider when ranking your website.
Growing your brand through social media requires some knowledge and several skills. It is also critical to understand which social media platforms can drive valuable traffic based on your niche so that you can focus your effort on the relevant channels.
For example, Pinterest and Instagram might drive the least external website visit in general, but they can be effective for specific topics like fashion and food-related content.
Last but not least, don’t forget to add referral links and calls to action (CTAs) to your profile and posts. Creating attractive CTAs with clear messages can help drive more traffic to your website.

9. Use Google Tools
Another important aspect of creating an SEO-friendly website is analyzing its core metrics. Website owners can get this information through various analytics tools, including Google Search Console and Google Analytics.
Don’t worry if you have a limited budget, as many of these tools are free.
Google Search Console can help website owners see how their sites are performing in Google search results.
The data can help you understand how Google views your content and which queries audiences use to find it. It gives you an overview of how much organic traffic you have generated and guides you on improving your website’s visibility based on Google’s guidelines.
This tool also provides detailed reports on any errors found in your website’s content and helps you identify various issues that might affect your search engine rankings. This includes problems like duplicate content, incorrect meta tags, or broken links.
While it’s not directly related to SEO, Google Analytics is also useful for giving you various metrics to help improve your site’s performance in general. For example, you can get the report on which page has the highest bounce rate.
This allows you to properly assess the possible cause of the problem and take the necessary steps to fix it.

10. Clean Up and Organize the Site Code
Your website consists of numerous lines of code that run various functions. These lines of code can become unorganized and hinder one another as you grow your website. To prevent this, we recommend cleaning them up when necessary.
This process can also help the search engine indexing process and make your site load faster. These two factors are the key elements that highly affect your website’s SEO performance.
Website code may cover different types of programming languages. The three most common ones are HTML, CSS, and JavaScript. Each of these languages is organized differently.
Fortunately, there are tools like Dirty Markup, HTML Cleaner, and JS Beautifier to help you with the process.

11. Add Internal Links
Internal linking is a process of adding hyperlinks within your content to other pages or posts on your website. This creates a web of interlinked content and helps search engines recognize the structure and relevance of each page.
You can add an internal link to elements like text, images, or buttons.
Consider the relevancy of each page and post you want to connect to ensure your internal links are effective. Put links on anchor texts that fit the appropriate context of the target pages to help smoothen the indexing process.
Strategic internal linking can also help reduce bounce rates. Visitors can find the right content and navigate the site more easily. Linking related other content on your blog posts also encourages visitors to explore and engage with your website more.
However, be careful not to overdo it. Inserting too many internal links can make your content look messy and negatively impact user experience.
Use tools like Internal Link Juicer, Link Whisper, and Yoast SEO to optimize your internal linking and improve the website’s SEO-friendliness.

12. Optimize the Title Tags and Meta Descriptions
Title tags and meta descriptions are HTML elements that give context to a page’s content. A title tag appears on the search engine result as clickable headlines, while a meta description offers short snippets about what readers can expect to find on the page.
While working on a title tag, ensure it includes the content’s focus keyword. Typically, it should align with the target audience’s search intent, helping your content appear on the right search result.
Keep your title tag between 50-60 characters. This will ensure they appear properly on the search results and have a higher chance of attracting readers.
On the other hand, a meta description gives you more space to introduce the content to potential readers. While a meta description’s length isn’t limited, remember that Google SERPs only show between 155-160 characters.
Each meta description should be unique and provide relevant information for your target audience. You may also include long-tail keywords to make it more search engine friendly.
Try to write a compelling copy for your meta description and show that your content provides value to the potential reader.

13. Use Images and Videos to Enhance the Content
Visual elements like images and videos can enrich your content and make it more appealing. Some visuals like graphs and charts also allow you to present data and communicate messages more effectively.
In addition to those benefits, adding images and videos to your content can also boost its SEO-friendliness. Media files allow your content to appear on the image and video tab of Google search results, improving its chances of getting clicks.
Your content can also appear as a rich snippet which shows more information and is more likely to appear at the top of the search results.
Remember to add optimized images and videos to maintain a fast-loading website. Optimizing images and videos involves compressing their size and adding the appropriate alt text.

14. Update Your Content Regularly
Creating new content regularly is a great SEO strategy. However, sometimes it may be difficult to come up with fresh content ideas. In these cases, you can update older content to improve your website’s SEO.
Changing between updating old content and creating new ones will keep people coming back to the site and also attract new visitors. Make sure you create content that fits the current issue to keep your target audience interested.
Don’t forget that implementing good SEO strategies is not enough if you don’t provide useful information to your visitors. Make sure to write good website content that brings value to your audience and helps build your brand reputation.

