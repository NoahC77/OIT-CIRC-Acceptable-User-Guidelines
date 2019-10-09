.. Unless specified otherwise by other comments within the rest of this document and delimited with ----- lines, the Acceptable User Guidelines are written by Dr. Perez. Excerpts from https://portal.tacc.utexas.edu/user-guides/stampede2#good-citizenship are used as well and noted when used.

=====================================
Acceptable User Guidelines
=====================================
OIT CI Research Computing (OIT-CIRC) resources are deployed, configured, and operated to serve a large, diverse user community. It is important that all users are aware of and abide by OIT-CIRC Usage Policies. Failure to do so may result in suspension or cancellation of the project and associated allocation and closure of all associated logins. Illegal transgressions will be addressed through University of Texas at Dallas (UT-D) and/or legal authorities.

Account Eligibility
===================
OIT-CIRC resources are available to faculty and staff at UT-Dallas, OIT-CIRC Research Partners, Texas higher educational institutions, and to US academic researchers. Additional supporting documentation may be required prior to accessing OIT-CIRC resources.

Eligible UT-Dallas, OIT-CIRC Partner, and Texas higher education users can request OIT-CIRC accounts. Individuals and groups that engage in collaborative research and development activities with UT-D are eligible to apply for user accounts.

Passwords 
=========
OIT-CIRC users must choose a strong password that should be unique to your OIT-CIRC username. Passwords (passphrases) for accounts should follow a model that results in fewer unintended lockouts for users.

Accounts (whether locally created through either computer or application, or through the NetID system) must follow the password (passphrase) requirements:

- Minumum password length: 12 characters
- Enforce maximum password age: 365 days
- Previous passwords must not be reused after being changed(Password history: 10 passwords)
- It should not contain NetID or your name
- It should include combinations of any 3 of the follow 4 complexities:
        1. uppercase letter
        2. lowercase letter
        3. number
        4. special character

- Number of allowed failed logon attempts: 25
- Reset failed login after: 60 minutes
- Accounts when locked out remain locked until removed by administrators or by users via self-service


Policies for OIT-CIRC Users
===========================
Users must abide by the following policies. Failure to do so will lead to disciplinary actions.

- Sharing of User Credentials is strictly prohibited
- Users are only allowed one account per person
- PI's are responsible for notifying OIT-CIRC when project users should be deactivated due to the departure of the user or termiantion of the project.
- Never infringe upon somone else's copyright. It is a violation of OIT-CIRC guidelines and federal law to participate in copyright infringement
- Never try to circumvent login procedures on any OIT-CIRC resource of otherwise attept to gain access where you are not allowed. NEver deliberately scan or probe any information resource without prior authorization.
- Computing reousrces may not be used for commercial purposes or personal gain.

Cryptocurrencies
----------------
Users are prohibited from running applications that mine cryptocurrency and/or use block-chain technology for personal gain. Violations of these guidelines will result in user's access to OIT-CIRC resources being terminated.

Use of Protected Software and Data
----------------------------------
PIs and users agree to NOT install or use any software or data that falls under the following protected categories International Traffic in Arms Regulations (ITAR), Export Administration Regulations (EAR), Health Insurance Portability and Accountability Act (HIPAA), Federal Information Security Management Act (FISMA), Personally Identifiable Information (PII), or any other protected control without first contacting issupport@utdallas.edu, an appropriate agreement Business Associate Agreement (BAA), Technology Control Plan (TCP), Memorandum Of Understanding (MOU), or other relevant agreements) between the UT-Dallas and the PI or home intuition must be in place before such software or data can be installed or used on any OIT-CIRC resource. Violations of these guidelines will result in the immediate removal of said software and/or data and deactivation of related projects, allocations, and user accounts.

Disciplinary Actions
--------------------
Punishment for infractions includes but is not limited to the following:

- Written or verbal warnings
- Revocation of access privilages to OIT-CIRC systems
- Termination of project(s) at OIT-CIRC
- Criminal Prosecution

.. This part is taken from https://portal.tacc.utexas.edu/user-guides/stampede2#good-citizenship

Be a Good Citizen
------------------------------

- **Know when your on a login node.** You can use your Linux prompt, the "hostname" command, or other mechanisms to do so.
- **Know what's appropriate on a login node.** A login node is a good place to edit and manage files, initiate file transfers, compile code, submit new jobs, and track existing jobs.
- **Avoid computationally intensive activity on login nodes.** This means
        - Dont run research applications on the login nodes; this includes frameworks like MATLAB and R.
        - Don't launch too many simultaneous processes: while it's fine to compile on a login node "make -j 16" (which compiles on 16 cores) may be a bit rude.
        - That script you wrote to check jobs status should probably do so every few minutes rather than serveral times a second.

Internal and External Networks
------------------------------

- **Avoid too many simultaneous file transfers.** You share the network bandwidth with oter users; don't use more than your fair share. Two or three concurrent sessions is probably fine. Twent is probably not.
- **Avoid recursive file transfers,** especially those involving many small files. Create a tar archive before transfers.

Submitting Jobs
---------------

- When you submit a job to the scheduler, **don't ask for more time than you really need.** The sscheduler wiil have an easier time finding a slot for the 2 hours you need than the 48 hours you request. This means the shorter queue wait times for you and everybody else.
- **Test your submission scripts.** Start small: make sure everything works on 2 nodes before you try 200. Work out submission bugs and kinks with 5 minute jobs that won't wait long in the queue and involve short, simple substitutes for your real workload: simple test problems; "hello world" codes; one-liners like "ibrun hostname"; or an ldd on your executable.
- **Respect memory  limits and other system onstraints.** If your application needs more memory than is available, your hob will fail, and may leave nodes in unusable states. Monitor your application's needs. Execute "module load remora" followed by "module help remora" for more information on a particularly handy monitoring tool.


.. --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Utilization
===========
OIT-CIRC has documented the purpose and proper use of resources and services via a series of
user guides and other web-based documents available on the OIT-CIRC web site. Users assume
the responsibility for becoming familiar with this documentation, particularly relating to issues
such as adherence to resource limits, proper and considerate use of the batch queuing system,
understanding the purpose and proper use of file systems and storage services, and proper use of
OIT-CIRC resources.

Use of OIT-CIRC resources should be used only for work directly related to the project for
which the resources were requested and granted. OIT-CIRC resources should only be used for
documented or obvious intended purpose.

The login or front-end nodes of the OIT-CIRC compute cluster(s) are reserved for compiling,
loading, and preparing to submit jobs to run in a batch queue. Running compute or I/O bound
processes on these nodes will cause excess overhead and affect the ability of the general user
community to use the systems effectively. Processes inappropriate to execute on these nodes will
automatically be killed and the user notified. Users repeatedly violating these guidelines will be
denied access to the system and must contact OIT-CIRC before access is restored.

The OIT-CIRC data storage resources are intended to provide the user community with a high-
speed, shared storage facility that is available to applications that span multiple OIT-CIRC
resources. Data stored on any OIT-CIRC data storage resource must be associated with research
projects approved by OIT-CIRC. Users storing data not meeting this criterion may lose all rights
to use OIT-CIRC resources. All users assume the responsibility for reading the information
contained in the appropriate system User Guide.

Account Deactivation Guidelines
===============================
Accounts will be deactivated for one of the following reasons:

- **PI Request** - An account deactivation request by a PI will result in the account being denied access to use the PI's project's allocation if the account does not have access to another active project.

- **Project Expiration** - Upon project expiration, all accounts (PI and user) will be immediately denied access to the allocation, and OIT-CIRC-issued user certificates will be revoked unless users have access to other active projects. All batch and remote job submissions will subsequently be rejected.

- **Violation of OIT-CIRC Guidelines** - Any user account determined by OIT-CIRC to be in violation of an OIT-CIRC guideline will immediately be denied access to all OIT-CIRC resources without notification.

- **Account Inactivity** - User accounts will be deactivated due to inactivity after 120 calendar days. This will be done automatically and users will have to submit a ticket to have their account reactivated. Any successful login to an OIT-CIRC resource (including the OIT-CIRC User Portal) will reset this timer.

Data Retention
==============
All data in /home and /work will remain on OIT-CIRC storage resources as long as the researcher is actively using the storage. Each user will be allocated 20GB of storage space on /home and this space will be backed up. Each research group will have 1TB of storage in /work. Storage space on /scratch is open to all users, however abuse of the /scratch resource will lead to disciplinary actions. To make the storage space more available to all campus users, all data stored in the OIT-CIRC /scratch area will be purged on a time-based basis according to the following schedule:

Every 30 days files larger than 5 TB will be purged.

Every 60 days files larger than 1 TB will be purged.

Every 180 days, all files will be purged.

If a group or PI requests more permanent storage, please send a message to ganymedeadmins@utdallas.edu to schedule an appointment to discuss purchasing more storage on OIT-CIRC high performance storage devices. User attempts to circumvent the file ages will face disciplinary actions

User Support
============
OIT-CIRC users are encouraged to request assitance from OIT-CIRC support when necessary. All requests for support must be submitted through email the OIT-CIRC email address ganymedeadmins@utdallas.edu. Exceptions to these guidelines will be handled on a case-by-case base. Special project collaborations are examples of situations requiring direct communication between OIT-CIRC and the user community.



.. This part is taken from https://portal.tacc.utexas.edu/user-guides/stampede2#good-citizenship

Help Desk Tickets
-----------------

- **Do your homework** before submitting a help desk ticket. What does the user guide and other documentation say? Search the internet for key phrases in your error logs; that's probably what the consultants answering your ticket are going to do. What have you changed since the last time your job succeeded?
- **Have realistic expectations.** Consultants can address system issues and answer questions, but they can't teach parallel programming in a ticket, and may know nothing about the package you downloaded. They may offer general advice that will help you build, debug, optimize, or modify your code, but you shouldn't expect them to do these things for you.
- **Describe your issue as precisely and completely as you can:** what you did, what happened, verbatim error messages, other meaningful output. When appropriate, include the information a consultant would need to find your artifacts and understand your workflow: e.g. the directory containg your build and/or job script; the modules you were using; relevant job numbers; and recent changes in your workflow that could affect or explin the behavior you're observing.
- **Be patient.** It may take a business day for a consultant to get back to you, especially if your issue is complex. It might take an exchange or two before you and the consultant are on the same page. If the admins disable your account, it's not punitive. When the file system is in danger of crashing or a login node hangs, they don't have tim to notify you before taking action.

.. --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

OIT-CIRC Citation
=================
Please reference OIT-CIRC in any research report, journal or publication that requires citation of any author's work. The recognition of the OIT-CIRC resources you used to perform research is important for acquiring funding for the next generation hardware, support services, and our

Research & Development activities in HPC, visualization, data storage, and grid infrastructure. The minimal content of a citation should include:

Office of Information Technology Cyber Infrastructure Research Computing (OIT-CIRC) The University of Texas at Dallas

Our suggested acknowledgement is 

The authors acknowledge the Office of Information Technology Cyber Infrastructure Research Computing (OIT-CIRC) at The University of Texas at Dallas for providing {HPC, visualization, services, or storage} resources that have contributed to the research results reported within this paper. URL: https://utdallas.edu/oit/departments/circ/ * Select one or more of the items within the braces, {}.

URL: https://utdallas.edu/oit/departments/circ/

* Select one or more of the items within the braces, {}.
