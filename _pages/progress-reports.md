---
layout: page
title: All Progress Reports
permalink: /progress-reports/ # Explicitly set permalink for clarity
---

## Grand Hotel Construction Progress Reports

Here you can find an archive of all weekly and monthly progress reports for the Grand Hotel construction project.

<ul class="report-list">
  {% assign sorted_reports = site.progress_reports | sort: "date" | reverse %}
  {% for report in sorted_reports %}
    <li>
      <a href="{{ report.url | relative_url }}">
        {{ report.title }}
        <span class="report-date">({{ report.date | date: "%B %d, %Y" }})</span>
      </a>
    </li>
  {% endfor %}
</ul>