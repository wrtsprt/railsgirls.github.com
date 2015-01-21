---
layout: default
title: Rails Girls App Tutorial - the other way around
permalink: app-top-down
---

# Rails Girls App Tutorial - Top Down

*Created by RailsGirls Brussels*

**Make sure you have Rails installed.** [**Follow the installation guide**](/install) to get set up.


## Get to know the tools

Should we keep that?

### Important

It is important that you select the instructions specific to your operating system - the commands you need to run on a Windows computer are slightly different to Mac or Linux. If you're having trouble check the Operating System switcher at the bottom of the commands. 

## *1.*Getting you started

In order to save time in the beginning and get right to the good stuff, you'll download a tiny app that we prepared for you.
(You can recreate it yourself if you want. We explain how to do it in the README). Just click this ???LINK??? and save the
file to computer. 

Now, let's open a terminal:

* Mac OS X: Open Spotlight, type *Terminal* and click the *Terminal* application.
* Windows: Click Start and look for *Command Prompt*, then click *Command Prompt with Ruby on Rails*.
* Linux (Ubuntu/Fedora): Search for *Terminal* on the dash and click *Terminal*.

Next, let's find the app in the terminal by running these commands:

<div class="os-specific">
  <div class="nix">
{% highlight sh %}
cd Downloads
cd railsgirls-app
{% endhighlight %}

    <div>
<p>You can verify that you landed in the correct directory by with the <code>ls</code> command. Running it should give you a result similar to the following:</p>
    </div>
	{% highlight sh %}
	??? rails app default directory listing ??? 
	{% endhighlight %}

    <div>
<p>Should that not be the case ask your guide to point you to the correct directory.</p>

<p>Now we can prepare the app and start the server as follows:</p>
    </div>

{% highlight sh %}
bundle install???
rake db:setup???
rails server
{% endhighlight %}
  </div>

  <div class="win">
<!-- ??? update windows paragraph accordingly, once we're done with the *nix version -->
{% highlight sh %}
mkdir projects
{% endhighlight %}

    <div>
<p>You can verify that a directory named <code>projects</code> was created by running the list command: <code>dir</code>. You should see the <code>projects</code> directory in the output. Now you want to change the directory you are currently in to the <code>projects</code> folder by running:</p>
    </div>

{% highlight sh %}
cd projects
{% endhighlight %}

    <div>
<p>You can verify you are now in an empty directory or folder by again running the <code>dir</code> command. Now you want to create a new app called <code>railsgirls</code> by running:</p>
    </div>

{% highlight sh %}
rails new railsgirls
{% endhighlight %}

    <div>
<p>This will create a new app in the folder <code>railsgirls</code>, so we again want to change the directory to be inside of our rails app by running:</p>
    </div>

{% highlight sh %}
cd railsgirls
{% endhighlight %}

    <div>
<p>If you run <code>dir</code> inside of the directory you should see folders such as <code>app</code> and <code>config</code>. You can then start the rails server by running:</p>
    </div>

{% highlight sh %}
rails server
{% endhighlight %}
  </div>
</div>

Open <http://localhost:3000> in your browser. 

You should see "Welcome friend." page, which means your app is up and running.

??? Should we do a little, what does it look like when the server is not running exercise here ???

## *2.*Creating a static HTML page

The welcome page you have just seen is a great example of a static HTML page served by a web server and then downloaded and displayed by your web browser. You will now see what such a page looks like in its raw form and learn how to make and change one. 

Open the file `app/views/welcome/index.html.erb` in your text editor. What you see here is mostly the text you find on the web page. But it is filled with a couple of special words and characters. Those are called HTML tags and markup the text to tell the browser how it should layout and show the page and contained text. 

Open your browser again and inspect the source code of the web page (??? instructions per OS / browser). Compare the what you see in the browser with what you see in your editor. What do you realise? Discuss with your peers and coach.

**Coach:** Discuss the findings.

Now let's change something in the HTML of the page. Go back to your editor for that and add ??? \<good idea here\>. Be sure to save the file in your editor, head over to the browser and reload the page. 

## *3.*From static to dynamic


## *4.*Advanced: MVC
## *5.*Advanced: Ruby in the Rails console 


## *6+.*What next?

* Add design using HTML &amp; CSS
* Add ratings
* Use CoffeeScript (or JavaScript) to add interaction
* Add picture resizing to make loading the pictures faster


## Where to go from here? 



# Stuff removed from the original guide, that we might reuse in a different order

Notice in this window the command prompt is not visible because you are now in the Rails server, the command prompt looks like this:

<div class="os-specific">
  <div class="nix">
{% highlight sh %}
$
{% endhighlight %}
  </div>
  <div class="win">
{% highlight sh %}
>
{% endhighlight %}
  </div>
</div>

When the command prompt is not visible you cannot execute new commands. If you try running `cd` or another command it will not work. To return to the normal command prompt:

Hit `CTRL-C` in the terminal to quit the server.

**Coach:** Explain what each command does. What was generated? What does the server do?
