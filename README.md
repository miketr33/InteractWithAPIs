# InteractWithAPIs
By Mike Tree
In this folder you will find my submission for the ‘Interact with APIs’ technical demo.
This submission includes two main folders. The first FullSolution contains the complete solution for this test. This includes an APIInteraction project folder which contains the main app code, as well as a UnitTests folder which contains a variety of unit tests, as well as one end-to-end integration test.
This project was created using .NET 6 (C#10) with Visual Studo for Mac (2022) (version 17.0.5 build 6). The APIInteraction references the newtonsoft library (https://www.newtonsoft.com/json) via NuGet package manager and the UnitTests are made using NUnit (https://nunit.org ).
The second folder contains the locally published CLI application, which you should be able to run by double clicking the APInteraction executable file.
If you have any trouble accessing either of these folders or their containing files, please don’t hesitate to get in touch via email. Unfortunately, I have not able to test these on a Windows PC as the only one I have available to me is my work machine. If required, I am more than happy to demo this application via a screen share video call.
Key Points:
- As part of a stretch goal I decided to use an alternative API for gathering the lyrics.
The Lyrics-Plus API (https://rapidapi.com/OsamaHu1277/api/lyrics-plus/) by OSMX retrieves the lyrics far quicker than the lyricsovh API, however it has restrictions on a free subscription. Therefore, I have restricted the number of requests made on each round to 5 requests. This can be easily changed by modifying the default value of the LyricApiLimit property in the Communications class. Please note that if the limit is reached (200 requests per month) the application may stop working. This can be overcome by setting up a paid subscription and changing the default header set at line 52 if Communications to match your subscription. I have ran a few tests using the current key and estimate there are around 185 requests remaining for this month.
    
