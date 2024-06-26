---
title: "2022 Online Meeting, December 6-8, 2022"
layout: event
breadcrumbs:
  - label: All Events
    link: '{{ site.root_url }}/events/'
  - label: 2022 Online Meeting
    link: '{{ site.root_url }}/event/2022/online-meeting/'
hero:
  image: ""
  subtitle: Join us to learn the latest about IIIF and help shape the future of the community.
  button:
    label: "Register"
    link: "https://stanford.zoom.us/meeting/register/tJcvceuuqTItG90yow4P0cusIHCBDp27UYiS"
---

<script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/jstimezonedetect/1.0.4/jstz.min.js"></script>
<!-- <script src="{{ site.root_url | absolute_url }}/js/vendor/add-to-calendar.min.js"></script>  -->
<script src="{{ site.root_url | absolute_url }}/js/vendor/moment-with-locales.min.js"></script>
<script src="{{ site.root_url | absolute_url }}/js/vendor/moment-timezone-with-data.js"></script> 

<script>
// var timezone = jstz.determine();
// var apiKey = 'AIzaSyBIB97V49ihYsXedQ0Ziw6s3SzcGf5G8z0';

// function text2id(text) {
//     return text.trim().toLowerCase().replace(/[:;,()]/g,'').replace(/[ ]/g,'-');
// }

// function loadEvents() {
//     // Initializes the client with the API key and the Translate API.
//     gapi.client.init({
//         'apiKey': apiKey,
//         // Discovery docs docs: https://developers.google.com/api-client-library/javascript/features/discovery
//         'discoveryDocs': ['https://www.googleapis.com/discovery/v1/apis/calendar/v3/rest'],
//     }).then(function () {
//         // Use Google's "apis-explorer" for research: https://developers.google.com/apis-explorer/#s/calendar/v3/
//         // Events: list API docs: https://developers.google.com/calendar/v3/reference/events/list
//         return gapi.client.calendar.events.list({
//             'calendarId': '1hnm5h86n94ore0vnoo188ter8@group.calendar.google.com',
//             'timeMin': '2022-12-06T01:00:00-00:00',
//             'timeMax': '2022-12-08T23:00:00-00:00',
//             'showDeleted': false,
//             'singleEvents': true,
//             'timeZone': timezone.name(), // This doesn't convert the timezone
//             'orderBy': 'startTime'
//         });
//     }).then(function (response) {
//         if (response.result.items) {
//             var days = {
//                 1: [],
//                 2: [],
//                 3: [],
//                 4: [],
//                 5: [],
//                 6: []
//             };
//             for (var i = 0; i < response.result.items.length; i++) {
//                 var day = moment(response.result.items[i].start.dateTime).day();
//                 if (response.result.items[i].summary.indexOf('- IIIF Online Meeting') != -1) {
//                     days[day].push(response.result.items[i]);
//                 }    
//             }   
//             var dayString = ['Monday, December 05', 'Tuesday, December 06', 'Wednesday, December 07', 'Thursday, December 08', 'Friday, December 09', 'Saturday, December 10'];
//             var content = '';
//             for (var i = 1; i < (dayString.length + 1); i++) {
//                 if (days[i].length > 0) {
//                     content += '<h2 id="' + text2id(dayString[i - 1].substring(0, dayString[i - 1].indexOf(','))) + '">' + dayString[i - 1] + '</h2><hr />';
//                     for (var j = 0; j < days[i].length; j++) {
//                         var event = days[i][j];
//                         content += '<h3 id="' + text2id(event.summary) + '">' + event.summary + '</h3>';
//                         content += '<b>' + moment(event.start.dateTime).format("LT") + ' - ' + moment(event.end.dateTime).format("LT") + ' ' + moment.tz.zone(moment.tz.guess()).abbr(new Date().getTime()) + '</b>';

//                         if (event.hasOwnProperty('location') && event.location.length > 0 && event.location.indexOf('register') != -1) {
//                             content += '<p class="register"><a href="' + event.location.trim() + '">Register</a></p>';
//                         }    

//                         if (event.hasOwnProperty('description') && event.description.length > 0) {
//                             content += '<p>' + event.description + '</p>';
//                         } else {
//                             content += '<p>Description to be added...</p>';
//                         }
//                     }
//                     content += '<br />';
//                     content += '<br />';
//                 }
//             }

//             var div = document.getElementById('schedule');
//             div.innerHTML = content;
//             anchors.add("#schedule h2, #schedule h3");
//         }
//     }, function (reason) {
//         console.log('Error: ' + reason.result.error.message);
//     });
// }
// function loadClient() {
//     gapi.load('client', loadEvents);
}

</script>

<script async defer src="https://apis.google.com/js/api.js" onload="this.onload=function(){};loadClient()" ></script>



**The 2022 Online Meeting will take place online December 6-8 and is free to attend.**

The Online Meeting is intended for a wide range of participants and interested parties, including digital image repository managers, content curators, software developers, scholars, and administrators at libraries, museums, cultural heritage institutions, software firms, and other organizations working with digital images and audio/visual materials.

As a counterpart to the IIIF in-person Annual Conference, this event is meant  both to introduce newcomers to IIIF and to provide a forum for discussion and dissemination for those with experience implementing and working with IIIF in a variety of contexts.

This event is guided by the [IIIF Code of Conduct][conduct].


## Logistics
* This event is free and open to all attendees.
* This event will be held using a single Zoom meeting for the sessions.  
* Presentations will be recorded. 
* All sessions will be in English unless otherwise noted.

## Registration
Registration is free! [Sign up once via Zoom](https://stanford.zoom.us/meeting/register/tJcvceuuqTItG90yow4P0cusIHCBDp27UYiS) and you'll have access to the Zoom meeting used for all sessions of the event. 

<div class="columns is-centered">{% include misc/button.html button_label="Register" button_link="https://stanford.zoom.us/meeting/register/tJcvceuuqTItG90yow4P0cusIHCBDp27UYiS" %}</div>

<h2>Schedule</h2>

### Full Event Calendar

The times on this calendar should adjust to your current time zone.
{:.no_toc}

<div id="calendar-container"></div>

<script>
  var timezone = jstz.determine();
  console.log('Name is ' + timezone.name());
  var pref = '<iframe src="https://calendar.google.com/calendar/b/1/embed?height=600&amp;wkst=2&amp;bgcolor=%23ffffff&amp;src=MWhubTVoODZuOTRvcmUwdm5vbzE4OHRlcjhAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ&amp;color=%23E67C73&amp;mode=WEEK&amp;tab=mc&amp;mode=week&dates=20221206/20221208&amp;title=IIIF%20Online%20Meeting&amp;ctz=';
  var suff = '" style="border:solid 1px #777; width: 100%; height: 600px;"></iframe>';
  //var pref = '<iframe src="https://www.google.com/calendar/embed?showPrint=0&amp;showCalendars=0&amp;mode=WEEK&amp;height=600&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=somecalendaridentifier%40group.calendar.google.com&amp;color=%23AB8B00&amp;ctz=';
  //var suff = '" style=" border-width:0 " width="800" height="600" frameborder="0" scrolling="no"></iframe>';
  var iframe_html = pref + timezone.name() + suff;
  document.getElementById('calendar-container').innerHTML = iframe_html;
</script>
<br>

<div id="schedule"></div>

## **Tuesday, December 06**

---

### **Newcomer Session: Introduction to the Community and Consortium -- IIIF Online Meeting**

Confused about the IIIF Community, or feel like you’re missing some information? Attend this session to learn how the IIIF community works. IIIF Consortium staff will talk about the different community groups and their various initiatives, approaches, and meetings. Come with questions!

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/ojOy9fWlBRk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### **Plenary: IIIF Community and Consortium Update -- IIIF Online Meeting**

The staff of the IIIF Consortium will welcome attendees and provide an update on where the IIIF community stands today, cover some important technical work and updates, and welcome attendees to the sessions over the next several days of meetings.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/eHe9MFadRTY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **Lightning Talks Part 1 -- IIIF Online Meeting**


* **An interoperable strategy for born digital**, Tom Crane, Digirati
* **Annotate for Research, Teaching and Learning**, Hiva Kadivar and Niqui O'Neill, North Carolina State University Libraries
* **Printing IIIF manifests with PDIIIF**, Chip Goines, Harvard University
* **Science in the Making: Using IIIF to showcase 350 years of scientific publishing**, Anne McLaughlin, The Royal Society, and Tristan Roddis / Cogapp Ltd
* **?as=iiif: An approach to a serverless API that returns search results as IIIF Collections**, Mat Jordan and Karen Shaw, Northwestern University Libraries
* **MLOL DH: IIIF-based digital libraries for Italian GLAMs**, Andrea Zanni and Raffaele Messuti, Horizons Unlimited H.u

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/WnAj4SBd3rs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **Design Community Group Showcase and Panel -- IIIF Online Meeting**

This 90 minute session will give panel participants and attendees the opportunity to think through and share ideas about how interface design can affect user experience, and how the IIIF community can work toward more consistent user experiences across different IIIF-enabled platforms. For those particularly interested in information architecture, usability, user experience, interaction design, and human-centered design, though all are welcome!

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/YmeKB7IxJS4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## **Wednesday, December 07**


---


### **The IIIF Commons and IIIF Prezi Projects -- IIIF Online Meeting**

[IIIF Commons](https://github.com/IIIF-Commons) is a growing community-supported effort to create high quality, reusable software components that can be used and reused as part of a more comprehensive IIIF solutions at any given institution. Join the leaders of this effort to find out more about how you can benefit from this collective work and also get involved.

[IIIF Prezi](https://github.com/iiif-prezi/iiif-prezi3)<span style="text-decoration:underline;"> </span>is a community-developed new version of a Python IIIF presentation library that makes it substantially easier to create and work with IIIF Presentation API 3.0 manifests in a variety of applications. Hear about the development process, including results from a community hackathon, as well details about how this library can be best used.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/chHe6Z2w53o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **From User Story to Specifications: How the IIIF Process Works, + Q&A with IIIF Specification Editors -- IIIF Online Meeting**

Ever wonder how suggestions and feedback from the community of IIIF implementers makes it all the way into official API specifications? Join the IIIF Specification Editors for an overview of the process that goes into crafting the[ six official IIIF APIs](https://iiif.io/api/index.html#current-specifications) and the various people and committees that provide feedback and governance during the process. 

Following the presentation the Editors will be available for a general Q&A.


<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/U1K3pHb2k68" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **IIIF 3D Showcase and Update -- IIIF Online Meeting**

Updates and developments of IIIF 3D will be shared by the Co-Chairs of the[ 3D Community group](https://iiif.io/community/groups/3d/) plus the[ 3D Technical Specification group](https://iiif.io/community/groups/3d/tsg/), and others in the community. There will be highlights of related projects, experiments, and discussions that are helping to evolve ideas and specifications for 3D interoperability and sustainability.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/0GPkj40ui1Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **Lightning Talks Part 2 -- IIIF Online Meeting**



* **IIIF Image API: Using IIPImage to Simultaneously Handle Multiple API versions**, Ruven Pillay, C2RMF
* **IIIF Presentation API 3.0 gateway for Kramerius digital library API**, Petr Žabička and Pavla Rychtářová, Moravian Library in Brno
* **Using WebAssembly to add scalability to IIIF**, Marcel Duin, Micrio
* **Evaluating the performance of htj2k images for IIIF**, Glen Robson, IIIF Consortium, Stefano Cossu, Harvard Library, Ruven Pillay (C2RMF/IIPImage, and Mike Smith, Kakadu Consultant
* **ETU 2.0, a netlify tool for the IIIF community**, Joe Song IntelliJourney.com

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/Zpd4w3QH_ew" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## **Thursday, December 08**

---


### **IIIF UK Regional event -- IIIF Online Meeting**

This will be a session to highlight the latest projects that are going on in the UK Agenda: https://docs.google.com/document/d/11yeKLZWSIZ4XG5xyCa3bh-BtY8H-xELfXH2E9gyIGcE/edit?usp=sharing


<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/XJDRBlsSBvk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### **IIIF Maps Showcase -- IIIF Online Meeting**

Join us for a showcase and discussion of geospatial and map-related possibilities in IIIF, including extensions for and use of the IIIF Presentation 3 API to support first class geospatial data. You will be introduced to members and projects in these communities as well as some of the technical aspects of combining geographic coordinates and IIIF resources.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/6Xb0i8ukSKk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### **Museums Group Session -- IIIF Online Meeting**

An hour-long session divided into two events:

**Museums showcase**: A lightning talk showcasing some of the innovative uses of IIIF by museums around the world

**Implementors roundtable**: A chance to talk about overcoming barriers to adoption at your institution, and to trade success stories. We will discuss things like image preparation workflow, file storage, serving images, producing manifests, supporting search and authentication.


<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/oGVbhyi2cew" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### **IIIF Consortium and Community Strategic Planning -- IIIF Online Meeting**

The Executive Committee of the IIIF Consortium will present the main pillars of work to help support the community and broaden the membership base that helps fund the work of the Consortium. Come ready to respond to and share ideas about high-value IIIF initiatives for the coming 3-5 years.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/5xGDbcwEtdU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Questions? Email us at <events@iiif.io>.

[iiif]: https://iiif.io/
[groups]: {{ site.url }}{{ site.baseurl }}/community/groups/
[consortium]: {{ site.url }}{{ site.baseurl }}/community/consortium/
[home-page]: http://iiif.io/
[iiif-discuss]: https://groups.google.com/forum/#!forum/iiif-discuss
[conduct]: {{ site.url }}{{ site.baseurl }}/event/conduct/
[hashtag]: https://twitter.com/search?q=%23iiif&src=typd
[twitter]: https://twitter.com/iiif_io
