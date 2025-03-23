---
title: Recent & Upcoming Talks
talks:
  - title: "Hugo Blox Builder Conference"
    event_url: "https://jovenes2025.rsme.es/index_en.html"
    location: "Hugo Blox Builder HQ, Bilbao, Spain"
    date: '2030-06-01T13:00:00Z'
    summary: "An example talk using Hugo Blox Builder's Markdown slides feature."
  - title: "Community Meetup"
    event_url: "https://community.example.com"
    location: "Community Center, Madrid, Spain"
    date: '2030-06-15T10:00:00Z'
    summary: "Join us for a community meetup discussing emerging web technologies."
  - title: "Tech Trends 2030"
    event_url: "https://techtalks.example.com"
    location: "Innovation Hub, Barcelona, Spain"
    date: '2030-07-20T14:00:00Z'
    summary: "A discussion on the future of technology and innovation."
---

## Upcoming Events and Recent Talks

<ul class="talks-list">
{{ range .Params.talks }}
  <li>
    <h3><a href="{{ .event_url }}">{{ .title }}</a></h3>
    <p>
      <strong>Date:</strong> {{ .date | dateFormat "January 2, 2006" }}<br>
      <strong>Location:</strong> {{ .location }}
    </p>
    <p>{{ .summary }}</p>
  </li>
{{ end }}
</ul>
