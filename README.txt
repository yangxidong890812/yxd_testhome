Welcome to ai-webdriver-1.0.11

Version completion time: 15/4 2020


With this tool, you don't need to write a line of code, just provide the simplest parameter (url) to start the UI intelligent exploration and testing journey.

Please install chrome browser before use

And configure the corresponding chromedriver.exe in the browserDrivers directory



Required parameters:


Specify the required parameters url and action in the config / compulsory_config file in the format:

Action = MakingBaseline
Url = https: //gitbook.cn/gitchat/author/5cea0bfbb78cc870612d8bba


This tool supports three actions:


MakingBaseline: The function is to intelligently grab all images on the page, and can also be used for non-testing purposes.

TestingBaseline: The function is to perform image exploration and image matching test on the specified URL according to the baseline image set

MakingAndTestingBaseline: The function is to execute TestingBaseline immediately after finishing MakingBaseline



Effect:


MakingBaseline: Generate a baseline picture collection in the current directory


TestingBaseline: conduct intelligent image comparison test based on baseline and generate screenshots & diffResults during the test,

Finally, generate testReport.txt test report in the current directory





Optional parameters:


You can configure optional parameters in config / optional_config (if you do not need to set the parameters, you can leave it blank):


UseMobileEmulation indicates whether to simulate mobile terminal operation (True is yes, False is no);

MouseHoverCssLocators indicates that you need ai-webdriver to try to hover and record the element css positioning method of the image, in English colon; separate positioning method (such as: li [name = 'following public number']; span [name = 'WeChat QR code '])

SearchDepth indicates the depth of exploration of ai-webdriver (recommended to be 1)



Run logs can be viewed in the logs folder.



Remarks: The program starts slower, but you do n’t need to worry about memory problems (theoretically, the memory usage usually does not exceed 100M) :)


Anti-virus software may report an error to chromedriver.exe, add trust or download it again.


The password will be updated at the end of each month, the password can be configured in config / secret_key, the latest password is regularly announced on the knowledge planet (AI测试前线)



If you have any requirements, please contact me:

email: 523314409@qq.com

QQ: 523314409

WeChat: shaoyuyishiwo

WeChat official account: AI测试前线