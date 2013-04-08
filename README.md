#Munin ip_conntrack check plugin

![tracking ip_conntrack count](https://raw.github.com/S1100/munin-plugin-ip_conntrack/master/sample.png)
<pre><code>
</code></pre>
* * *
##INSTALLATION

###1. get the file
<pre><code>
# cd /usr/share/munin/plugins/
# wget https://raw.github.com/S1100/munin-plugin-ip_conntrack/master/ip_conntrack
# chmod 755 ip_conntrack
# cd /etc/munin/plugins
# ln -s /usr/share/munin/plugins/ip_conntrack .

</code></pre>

###2. check the response
<pre><code>
#  time munin-run ip_conntrack 
max_ip_conntrack.value 524288
used_ip_conntrack.value 171743

real    0m0.056s
user    0m0.047s
sys     0m0.010s
</code></pre>
If your server needs over 5 second, should not to use this plugin.

###3. No problem, then
<pre><code>
# service munin-node restart
</code></pre>
