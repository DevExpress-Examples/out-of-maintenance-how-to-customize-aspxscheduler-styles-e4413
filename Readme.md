<!-- default file list -->
*Files to look at*:

* [Default.aspx](./CS/WebSite/Default.aspx) (VB: [Default.aspx.vb](./VB/WebSite/Default.aspx.vb))
* [Default.aspx.cs](./CS/WebSite/Default.aspx.cs) (VB: [Default.aspx.vb](./VB/WebSite/Default.aspx.vb))
<!-- default file list end -->
# How to customize ASPxScheduler styles


<p><strong>Problem:</strong></p><p><br />
I have read several topics from the <a href="http://documentation.devexpress.com/#AspNet/CustomDocument11689"><u>Appearance Customization - Theming</u></a> help section. I still do not understand how to correctly apply one of the <a href="http://documentation.devexpress.com/#AspNet/CustomDocument6655"><u>Available Themes</u></a> to the <a href="http://documentation.devexpress.com/#AspNet/clsDevExpressWebASPxSchedulerASPxSchedulertopic"><u>ASPxScheduler</u></a> control and still have the capability to customize individual theme parts, i. e., <a href="http://documentation.devexpress.com/#AspNet/CustomDocument7211"><u>sprites</u></a> and a regular CSS settings.<br />
</p><p><strong>Solution:</strong><strong><br />
</strong></p><p>You can use the <a href="http://documentation.devexpress.com/#ASPxThemeDeployer/CustomDocument5500"><u>ASPxThemeDeployer</u></a> tool to copy one of the predefined themes into your web site and modify theme elements according to your requirements. Here are the detailed steps:</p><p>1) Run the ASPxThemeDeployer tool and copy particular theme (e.g., "Office2010Blue") files for <strong>ASPxScheduler </strong>and <strong>ASPxEditors </strong>products into a web site folder.<br />
2) Set the <a href="http://documentation.devexpress.com/#AspNet/CustomDocument7013"><u>enableThemesAssembly</u></a> option to false in a <strong>web.config</strong> file.<br />
3) Apply a theme to your website by using the approach from the "Applying a Theme" section of the <a href="http://documentation.devexpress.com/#AspNet/CustomDocument11725"><u>Apply a Theme with the ASP.NET Mechanism</u></a> help article (e.g., define it in the <strong>web.config</strong> file).<br />
4) Run the website and make sure that the theme is applied.<br />
5) Use the approach from the <a href="https://www.devexpress.com/Support/Center/p/K18570">How to inspect CSS rules</a> KB article to determine which CSS names have the <a href="http://documentation.devexpress.com/#AspNet/CustomDocument3830"><u>ASPxScheduler visual elements</u></a> you wish to customize. Here is an example:</p><p><img src="https://raw.githubusercontent.com/DevExpress-Examples/how-to-customize-aspxscheduler-styles-e4413/12.2.11+/media/7d87630e-9d00-47b6-b88d-33b67e56f3f4.png"></p><p>6) Find the corresponding CSS rules in the <strong>~/App_Themes/<Your_theme_name>/Scheduler/styles.css</strong> file and modify them.<br />
7) Run the website again and make sure that your changes have been applied.</p>

<br/>


