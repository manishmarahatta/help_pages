
<!--
.. title: Bug Bounty
.. slug: BugBounty
.. date: 2016-11-28
.. tags:
.. category:
.. link:
.. description:
.. type: text
-->


PythonAnywhere offers a bounty for responsibly disclosed bugs. We determine the
payout depending on the severity and impact of the submitted bug. We only pay
out on the first report of a particular issue, so it's best if you contact us
first to see whether we're already working on something.

## Bug classes we're not really interested in
* "I can run code on your servers" - Yup. That's our business.
* Self XSS - If you can execute XSS-style attacks against your own account by
  uploading a file and then loading it in the browser, that's not particularly
  interesting to us.
* Auto-pwnage - "If I run this code it does something bad to my
  account/files/web apps"
  
## Bug classes we're interested in
* General XSS, CSRF etc. - Can you get a user that is logged in to PythonAnywhere to do
  something malicious to their own account by e.g. having them follow a link?
* Cross-user exploits - Can you do something bad to another user on PythonAnywhere
  from your account? Unless you're a teacher doing something malicious to your
  students - there's an explicit trust relationship, there.
* Information leakage - Can you learn something private (see their files,
  access account information) about another user/account registered on
  PythonAnywhere?
  
## Bug classes we're very interested in
* Session/cookie hijacking
* Privilege escalation in consoles, web apps and scheduled tasks
* Sandbox escape in consoles, web apps and scheduled tasks
