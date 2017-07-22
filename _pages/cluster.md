---
permalink: /cluster/
layout: splash
title: "Tips and tricks for the cluster"
header:
  overlay_color: "#5e616c"
  overlay_image: sixPtRelations.jpg
  overlay_filter: .4
  caption: ""
author_profile: false
---

# Setting up dropbox

Follow the instructions [here](https://www.dropbox.com/install-linux).  i.e. you will want to:
   1. execute `` cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf ``
   2. execute ``~ /.dropbox-dist/dropboxd ``
   3. Download the python script at put it somewhere handy

# Getting to qft from home.

  1. First login to scylla.extra.cea.fr or charybde.extra.cea.fr.
  2. Goto headnode (qft1)
  3. If you need an intereactive shell use ``qsub -I`` otherwise submit batch jobs.

# Queuing system

  1. We use Torque / Maui .
  2. Documentation  [here](http://docs.adaptivecomputing.com/torque/6-1-1/adminGuide/help.htm#topics/torque/2-jobs/submittingManagingJobs.htm%3FTocPath%3D3%2520Submitting%2520and%2520Managing%2520Jobs%7C_____0).

# Screen

  1. charybde and scylla are literally restarted once a week. (??)
  2. Learn to use screen.
      a.  man page: [here](https://www.gnu.org/software/screen/manual/screen.html#Concept-Index)
      b.  some tutorials:   [here](https://www.rackaid.com/blog/linux-screen-tutorial-and-how-to/) and [here](https://www.mattcutts.com/blog/a-quick-tutorial-on-screen/)

# ssh-keygen
  * Learn how to use [ssh](https://www.digitalocean.com/community/tutorials/ssh-essentials-working-with-ssh-servers-clients-and-keys).
