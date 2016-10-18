# HtmlArray
Combined with the front end of the way HTML page, a combination of static page fast program.

### [Simple Example](https://github.com/dingdong-io/HtmlArray/blob/master/examples/easy.html)
Core code 

    <script type="text/javascript" src="other/jquery-2.1.4.min.js"></script>
    <script  type="text/javascript" src="../HtmlArray.js"></script>
    <script>
      HtmlArray = [
        "module/header/header.html",
        "module/footer/footer.html",
      ];
    </script>
1 introduce dependency jQuery
2 the introduction of HtmlArray
3 define the HtmlArray array, each sub page of the path (string format) collection.
Well, open the page to see it, is so simple.
If there is anything else to say, the path needs to be local, do not allow cross domain, write a ` http://example.com 'is invalid (unless you are the station webmaster)
  
### [Parameter example](https://github.com/dingdong-io/HtmlArray/blob/master/examples/AllConfig.html)
  !!To be added

### Use environment
　　The original intention of the project is to use a pure front end of the way to mix the page, and even allows the front end engineers do not need to build the server.

*  Scope of application
Quick combination page, especially suitable for front end Engineer
!! To be added 
  
* Don't build server
Of course, this time you can only open in the local, but need to do one step, you can [reference here] (http://blog.sina.com.cn/s/blog_a76aa1590101eams.html). Right - click on the shortcut to chrome - target - in the back of the original field and add "--allow-file-access-from-files".
The method is effective for chrome, other WebKit kernel browser is also available, such as the domestic dual core browser settings in the speed mode is effective, compatible mode error.
Measured, the need to turn off the chrome, waiting for the browser process all closed, and then the shortcut to open.
  
*  Open server
Of course, as a web worker, I still recommend that you open the server, are static pages, IIS/apache are competent. Next, you will not limit the IE/ browser, Firefox is OK, you can also other devices in the LAN, including mobile phone access to it.
Of course, the binding domain name, the public can also visit.
  
In spite of this, it should be used to help the front end engineer to mix the page, and should not be used in the back-end。
  
  
##### Project.
Cause is the company's project using modular design, the head, the bottom, the main body, the sub module, respectively, there are several templates, the back-end and then put them into a complete page.
On the one hand, the front needs to be combined with the page manually, to ensure that the style, the script in the combination page to submit to the back end. On the other hand, with the increasing number of sub modules and combination pages, the maintenance of more trouble, a sub module of the changes, all of the reference to its composite surface need to change, so the idea of the combination of the germination page. (but no backend experience is determined by JS).
  
##  
###FAQ  
######Why not use iframe?
Iframe to save more, but now the page is seldom used, in order to simulate the real portfolio page, do not use it. If the two script conflict, but because of the use of iframe did not find them out, page the purpose of combination will be greatly reduced.
Later may add the parameters of the iframe to help cross domain load, but there is no need for this.


