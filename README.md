# AWS-Projects
Collection of AWS projects

Project 1 - Hosting a website on AWS

* Step 1 : Navigate to AWS Console page
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/07dd61b0-83bb-49d5-ac49-a6a5f54d7bf3)

* Step 2 : Domain Registration - Open Route 53 (You can do this by typing Route 53 in the search bar)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/d0b8feee-c54d-41c0-bb36-980fe89956cd)

    Click Register Domain button, here you can search for a domain name. Adding .click instead of .com is usually the cheapest option ($3).
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/379cbe64-6264-4021-adca-384ea076cd48)

    Scroll down and follow to the next steps and complete the checkout. For test purposes you can turn off Auto-renew.
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/2b9ab413-3cf8-4cc5-982d-e70ea601147c)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/5a4d8773-148f-4c61-8be4-9c69793a4d75)

* Step 3: Open S3 (You can do this by typing S3 in the search bar)and click create Bucket. Give the bucket the same name as your domain. Select a Region close to you to prevent latency issues.
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/5f0ff192-cb65-4143-b6dd-39bbe3139d15)

    Unclick block all public access as this is a public facing website
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/4d781696-3d59-4f15-b528-966e27c78e71)

    Click disable Bucket versioning. Click Server-side encryption with AWS S3 managed keys. Click Enable Bucket keys then Create Bucket
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/316423ec-c87b-4a7f-a2a2-57b35f3df46c)

    Successful Bucket creation! Click on your Bucket under Name column to go into the Bucket and begin uploads.
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/02c756f9-d183-4df9-89e8-213859768efd)

* Step 4: Uploads - Click the yellow Upload button 
 ![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/4d8b5cc3-4e68-4640-bde6-9d1af0868331)

    Click Add files to open your file explorer and locate the files for your website. Depending on how your website is put together this might be something simple like an index.html file or could contain more files, then click Upload at the bottom of the page.
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/ab6a8115-153d-4298-85e9-26ccb88f75b1)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/2ab29af0-e229-4df2-bab8-5ac818916725)


* Step 5: Properties & Permissions
  
  Click the Close button at the top of the page to navigaate back to the Bucket, click the Properties tab and scroll down to Static website hosting, click Edit and Enable Web hosting
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/7a87b52d-4dd9-48cb-a69d-17f6708145dd)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/acf86801-ee27-48d6-af01-6db5fa62b2b6)
  At the Index Document section, specify the Home page for your website, then click Save changes
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/b9c9bc42-965b-4809-b9eb-c31f0fbad1be)

  Move to the Permissions tab and scroll down to the Bucket Policy - Edit Policy
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/27d5539e-4a86-4376-8e2f-858303e28bef)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/daec8523-fa38-495f-80ee-3cf3ad537baf)

  Here you need to add in the information from the S3 Bucket policy.txt file and swap out the BUCKET-NAME for the name of your bucket, click Save changes
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/a2c646d2-3d06-4f87-9c81-a9057a9327df)

Click on the Objects tab and open your index.html file, then click Open in the top of the screen to see your website being hosted on AWS S3.
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/53165d85-7882-4afa-8138-f1f2ed0d862b)
![image](https://github.com/Rocket387/AWS-Projects/assets/66258779/50ab1ce0-cb7a-4ddc-bff5-2cadfba445e7)

A step up from this is to redirect the domain name to the S3 Bucket so the website name can be seen in the address bar rather than s3.eu-amazon.west........








