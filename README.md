<table border=0>
  <tr>
    <td valign="top"><h1>WebCL_Outline</h1>
      An image processor utilizing WebCL.<br />
      Written by Mark Becker
      <hr>
      <ul>
        <font size='4'><b>Project description</b></font>
        <ul>
          <li>This project was created to explore the usage of the newly developed specification WebCL.
          <li>It was created as a preliminary project for the larger, more complex project <a href="https://github.com/markbecker/WebCL_Raytracer" target=blank>WebCL_Raytracer</a>.
          <li>The kernel used in this project finds the edges of a given image file.
          <li>Like OpenCL, WebCL allows for direct access to the many-core environment of the CPU <br />
          and or GPU.
          <li>An image processor was developed and used to demonstrate the power of parallelization.<br />
        </ul>
        <br/>
        <font size='4'><b>Developed and tested on...</b></font>
        <ul>
          <li>Mark's Desktop:
            <ul>
              <li>OS - Windows 7 Professional 64-bit
              <li>CPU - Intel Core i5 760 @ 2.80GHz
              <li>MB - ASUS P7P55D-E Pro
              <li>VC - ATI Radeon HD 5750
              <li>AMD App Acceleration SDK
              <li>Intel SDK for OpenCL
            </ul>
        </ul>
      </ul>
      <hr>
      <ul>
        <font size='4'><b>Runtime Environment</b></font><br />
        <ol>
          The easy part...
          <li>This web application can only be run on Firefox browser<br />
          <li>The Nokia WebCL extension needs to be installed<br />
          <li>WebGL needs to be enabled<br />
          <li>WebCL needs to be enabled<br />
            All of this can be checked and or installed at <a href="http://webcl.nokiaresearch.com/index.html" target=blank>Nokia Research</a><br />
            <br />
            The not as easy part...<br />
          <li>AMD App Acceleration SDK installed - <a href="http://developer.amd.com/sdks/AMDAPPSDK/Pages/default.aspx" target="_blank">AMD Developer Central</a><br />
          <li>Intel SDK for OpenCL installed - <a href="http://software.intel.com/en-us/articles/vcsource-tools-opencl-sdk/" target="_blank">Intel SDK for OpenCL</a><br />
            <br />
            The <a href="http://webcl.nokiaresearch.com/faq.html" target="_blank">FAQ</a> for Nokia Research's WebCL
        </ol>
      </ul>
      <ul>
        <font size='4'><b>Runtime Environment Concerns</b></font>
        <ul>
          <li> This application runs directly on the GPU or CPU. With that in mind, pushing the adjustments,<br />
            size, run count, may effect the computer it is run on. There was more than a few times that<br />
            during development the GPU was overflowed and needed to restart. It also may push the limits<br />
            of Firefox.
          <li> Therefore, a certain amount of caution needs to be used. But don't be afraid to use it.
        </ul>
      </ul>
      <hr>
      <table width="810" border="0" cellpadding="2" cellspacing="0">
        <tr>
          <td width="470" valign="top"><ul>
              <font size='4'><b>Web Page Interface</b></font>
            </ul></td>
          <td width="340" valign="top">&nbsp;</td>
        </tr>
        <tr>
          <td valign="top" colspan="2">Screen shot of page displayed:<br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot1.png" target=blank><img border=1 src="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot1.png" width="800" height="599" alt="Screenshot 1"/></a><br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot1.png" target=blank>Click for larger</a><br />
            <br /></td>
        </tr>
        <tr>
          <td width="470" valign="top"><ul>
              <font size='4'><b>Choose Images:</b></font><br />
              <ul>
                <li> There is two images to choose from to outline. Each image is of different size. With the increase in size comes an increase in run-time.
              </ul>
            </ul><ul>
              <font size='4'><b>Choose Device:</b></font><br />
              <ul>
                <li>The page creates a list of appropriate platforms and devices that can be used with the WebCL kernel.
                <li>Shown is both the Intel and AMD implementation of OpenCL.
              </ul>
            </ul><ul>
              <font size='4'><b>Information Output:</b></font><br />
              <ul>
                <li> The 'Information Output' is created after each run. The text is labeled to be self explanatory. Some of the information presented is based on the environment the code (kernel) is run on. The other info is specifically concerning the individual run.
              </ul>
            </ul></td>
          <td width="340" valign="top">Choose Device input section:<br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot2.png" target=blank> <img border=1 src="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot2.png" width="332" height="659" alt="Screenshot 2"/></a><br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot2.png" target=blank>Click for raw image</a><br /></td>
        </tr>
        <tr>
          <td width="470" valign="top"><ul>
              <font size='4'><b>Scene Created:</b></font><br />
              <ul>
                <li> The largest section of the page is reserved for a displaying of the processed image created. The area is fixed to display a 800 by 600 image. Larger (and smaller) images can be created and scroll bars will be implemented accordingly.
              </ul>
            </ul></td>
          <td width="340" valign="top">Choose Image input section:<br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot3.png" target=blank> <img border=1 src="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot3.png" width="334" height="264" alt="Screenshot 3"/></a><br />
            <a href="https://github.com/markbecker/WebCL_Outline/raw/master/Graphics/screenshot3.png" target=blank>Click for larger image</a><br /></td>
        </tr>
      </table>
      <hr>
      <ul>        
        <font size='4'><b>What is WebCL?</b></font>
        <ul>
          The WebCL working group is working to define a JavaScript binding to the Khronos OpenCL <br />
          standard for heterogeneous parallel computing. WebCL will enable web applications to <br />
          harness GPU and multi-core CPU parallel processing from within a Web browser, enabling <br />
          significant acceleration of applications such as image and video processing and advanced <br />
          physics for WebGL games.<br />
          <li><a href="http://www.khronos.org/webcl/" target=blank>More info from Khronos</a>
        </ul>
        <br/>
        <font size='4'><b>What is Nokia Research doing?</b></font>
        <ul>
          Nokia Research has developed an extension for the Firefox web browser running on<br />
          Windows and 32-bit Linux.<br />
          <li><a href="http://webcl.nokiaresearch.com/index.html" target=blank>More info from Nokia Research</a>
        </ul>
      </ul>
      <hr></td>
  </tr>
</table>
