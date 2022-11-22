# How to Get Involved

This page contains links to all of the meeting notes, design docs and related discussions around the different APIs managed by the Multicluster SIG.

## Feedback and Questions

For general feedback, questions or to share ideas please feel free to [create a
new discussion][gh-disc].
[gh-disc]:https://github.com/kubernetes-sigs/gateway-api/discussions/new

## Bug Reports

Bug reports should be filed as [Github Issues][gh-issues] on this repo.

**NOTE**: If you're reporting a bug that applies to a specific implementation of
Multicluster API and not the API specification itself, please check our
[implementations page][implementations] to find links to the repositories where
you can get help with your specific implementation.

[gh-issues]: https://github.com/kubernetes/community/labels/sig%2Fmulticluster
[implementations]: ../implementations.md

## Communications

Major discussions and notifications will be sent on the [SIG-MC mailing
list][signetg].

We also have a [Slack channel (sig-multicluster)][slack] on k8s.io for day-to-day questions, discussions.

[signetg]: https://groups.google.com/forum/#!forum/kubernetes-sig-multicluster
[slack]: https://kubernetes.slack.com/archives/C09R1PJR3

## Meetings

Meetings discussing the evolution of the different APIs on SIG-Multicluster happen bi-weekly on Tuesdays at 9:30AM Pacific Time / 18:30 CET. Join kubernetes-sig-multicluster@googlegroups.com to get a calendar invite. 

<iframe
  src="https://calendar.google.com/calendar/embed?src=88fe1l3qfn2b6r11k8um5am76c%40group.calendar.google.com"
  style="border: 0" width="800" height="600" frameborder="0"
  scrolling="no">
</iframe>

* [Zoom link](https://zoom.us/my/k8s.mc)
* [Convert to your timezone](http://www.thetimezoneconverter.com/?t=15:00&tz=PT%20%28Pacific%20Time%29)
* [Add to your calendar](https://calendar.google.com/event?action=TEMPLATE&tmeid=NXU4OXYyY2pqNzEzYzUwYnVsYmZwdXJzZDlfMjAyMTA1MTBUMjIwMDAwWiA4OGZlMWwzcWZuMmI2cjExazh1bTVhbTc2Y0Bn&tmsrc=88fe1l3qfn2b6r11k8um5am76c%40group.calendar.google.com&scp=ALL)


### Meeting Notes and Recordings

Meeting agendas and notes are maintained in the [meeting notes
doc][meeting-notes]. Feel free to add topics for discussion at an upcoming
meeting.

All meetings are recorded and automatically uploaded to the [SIG Multicluster meetings Youtube playlist][sig-multicluster-yt-playlist].

#### Archived Notes
Some documents from previous quarters were uploaded [here][sig-mc-previous-quarters-docs].

[sig-mc-previous-quarters-docs]: https://drive.google.com/open?id=0B6O6mvmXbHiFRE03d0FPSGtTSG8

#### Initial Design Discussions


* [Kubecon 2019 San Diego: API evolution design discussion][kubecon-2019-na-design-discussion]
* [SIG-NETWORK: Ingress Evolution Sync][sig-net-2019-11-sync]
* [Kubecon 2019 Barcelona: SIG-NETWORK discussion (general topics, includes V2)][kubecon-2019-eu-discussion]

[sig-multicluster-yt-playlist]: https://www.youtube.com/playlist?list=PL69nYSiGNLP0HqgyqTby6HlDEz7i1mb0-
[sig-net-yt-playlist]: https://www.youtube.com/playlist?list=PL69nYSiGNLP2E8vmnqo5MwPOY25sDWIxb
[early-yt-playlist]: https://www.youtube.com/playlist?list=PL7KjrPTDcs4Xe6SZj-51WvBfufKf-la1O
[kubecon-2019-na-design-discussion]: https://docs.google.com/document/d/1l_SsVPLMBZ7lm_T4u7ZDBceTTUY71-iEQUPWeOdTAxM/preview
[kubecon-2019-eu-discussion]: https://docs.google.com/document/d/1n8AaDiPXyZHTosm1dscWhzpbcZklP3vd11fA6L6ajlY/preview
[sig-net-2019-11-sync]: https://docs.google.com/document/d/1AqBaxNX0uS0fb_fSpVL9c8TmaSP7RYkWO8U_SdJH67k/preview
[meeting-notes]: https://tinyurl.com/sig-multicluster-notes

## Presentations and Talks

Kubecon NA 2022 update slides and video
AWS based demo combining About API and their MCS implementation with AWS CloudMap controller
Kubecon EU 2022 video and slides
Demo on mutlicluster plugin for coredns
Kubecon NA 2021 video and slides
Explanation of MCS, mutlicluster DNS
Here Be Services video and slides
Demo of MCS on GKE and Submariner.io


| Date           | Title |    |
|----------------|-------|----|
| October, 2022 | [Kubecon 2022 Detroit: SIG Multicluster Intro & Deep Dive][2022-kubecon-2022-detroit-schedule] | [slides][2019-kubecon-na-slides], [video][2019-kubecon-na-video]|
| November, 2019 | Kubecon 2019 San Diego: SIG-NETWORK Service/Ingress Evolution Discussion | [slides][2019-kubecon-na-community-slides] |
| May, 2019      | [Kubecon 2019 Barcelona: Ingress V2 and Multicluster Services][2019-kubecon-eu] | [slides][2019-kubecon-eu-slides], [video][2019-kubecon-eu-video]|
| March, 2018    | SIG-NETWORK: Ingress user survey | [data][survey-data], [slides][survey-slides] |

[2022-kubecon-2022-detroit-schedule]: https://sched.co/182P2
[2019-kubecon-na-slides]: https://static.sched.com/hosted_files/kccncna19/a5/Kubecon%20San%20Diego%202019%20-%20Evolving%20the%20Kubernetes%20Ingress%20APIs%20to%20GA%20and%20Beyond%20%5BPUBLIC%5D.pdf
[2019-kubecon-na-video]: https://www.youtube.com/watch?v=cduG0FrjdJA
[2019-kubecon-eu]: https://kccnceu19.sched.com/event/MPb6/ingress-v2-and-multicluster-services-rohit-ramkumar-bowei-du-google
[2019-kubecon-eu-slides]: https://static.sched.com/hosted_files/kccnceu19/97/%5Bwith%20speaker%20notes%5D%20Kubecon%20EU%202019_%20Ingress%20V2%20%26%20Multi-Cluster%20Services.pdf
[2019-kubecon-eu-video]: https://www.youtube.com/watch?v=Ne9UJL6irXY&t=1s
[survey-data]: https://github.com/bowei/k8s-ingress-survey-2018
[survey-slides]: https://github.com/bowei/k8s-ingress-survey-2018/blob/master/survey.pdf
[2019-kubecon-na-community-slides]: https://docs.google.com/presentation/d/1s0scrQCCFLJMVjjGXGQHoV6_4OIZkaIGjwj4wpUUJ7M

## Code of conduct

Participation in the Kubernetes community is governed by the [Kubernetes Code of
Conduct](https://github.com/kubernetes/community/blob/master/code-of-conduct.md)
