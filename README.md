<h4>Learning Goals</h4>
  <ul>
    <li>To study and understand the implementation of the DNS
      protocol.</li>
    <li>To learn how to read and implement a well specified
      protocol.</li>
    <li>To improve your programming and debugging skills as they
      relate to the use of binary data in Java.</li>
    <li>To develop an understanding of how to send and receive binary
      data.</li>
  </ul>
  
  <h4>Assignment Overview</h4>
  <p>This is the first part of the second programming assignment.  In this
  part, you will learn about the format of DNS messages and write code to
  encode and decode these messages.  In the second part, you will use this
  code to implement a DNS client program similar to dig or nslookup.</p>
  <p>As in the
    previous assignment you will complete specific sections of an
    existing application that already provides the UI functionality
    (via a command-line interface). You are responsible for
    implementing the encoding and decoding according to the DNS protocol.</p>
  <p>To start your assignment, download the
    file <a href="/pl/course_instance/2374/instance_question/17082889/clientFilesQuestion/DNSMessage.zip" download="">DNSMessage.zip</a>. This
    file contains a directory called <code>DNSMessage</code>
    which can be imported into IDEs like IntelliJ or Eclipse to
    develop your code.</p>
  <p>The file above contains a skeleton code that provides a
    console-based user-interface for the functionality you are to
    implement. The interface, exercises methods in the DNSMessage class that
    you will complete.
    More specifically, you will need to
    implement the code that performs each of the following tasks:</p>
  <ul>
    <li>Implement methods that allow a received DNS message to be decoded
      and interpreted.</li>
    <li>Implement methods that allow a DNS message to be constructed in
      preparation for sending.
      response.</li>
  </ul>
  <p>Remember, you are only required to implement a subset of the
    capabilities of a DNS message, so some of the material in the references
    goes beyond what you need. Keep in mind that the RFC describes the data
    (protocol) exchanges between the DNS client (i.e., what you are
    writing) and a DNS nameserver.</p>
  <p>All the functionality listed below is based on the implementation
    of the constructor and methods of the
    class <code>ca.ubc.cs.cs317.dnslookup.DNSMessage</code>,
    available in the provided code. This is the only file you are
    allowed to change.</p>
  <p><strong>You are not permitted to use any built-in or Java library
    methods to convert domain names to IP addresses</strong>. While
    the provided code uses the <code>getByName()</code> method
    of <code>InetAddress</code> to convert a string to its
    corresponding IP address, it should not be used in any other
    context except to convert a dotted-decimal IPv4 address (e.g.,
    199.7.83.42) or a hex-encoded IPv6 address (e.g.,
    2607:f8b0:400a:806::2003) to its corresponding <code>InetAddress</code>
    object. You can also use <code>InetAddress.getByAddress()</code>
    to convert an IP address to its string representation
    (dotted-decimal or IPv6-based). 
