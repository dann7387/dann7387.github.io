---
title: Vagrantfile Cheat Sheet
author: Danny Cheung
tags:
  - vagrant
  - cheat sheet
---

# Basic Vagrantfile


{% capture basic_vagrantfile %}{% highlight ruby %}
# Need to specify that we are using Varant v2
VAGRANTFILE_API_VERSION = '2'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = '<box_name>'

  config.vm.provider :virtualbox do |vb|
    # Run VM in headless mode
    vb.gui = false

    # RAM in MB
    vb.memory = 1024

    # Number of CPUs
    vb.cpus = 1
  end
end
{% endhighlight %}
{% endcapture %}

{{ basic_vagrantfile | markdownify }}

# Include config from another file

{% highlight ruby %}
load '<External_File>'
{% endhighlight %}

