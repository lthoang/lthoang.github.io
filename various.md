---
layout: default
title: Various
permalink: /various/
---

<h3 class="home-section__header">Research Grant</h3>
- <div class="grant-item">Title: Trustworthy AI for Ranking Systems: Foundations and Applications. Source: NAFOSTED (102.01-2025.66), Vietnam. Grant: 1,350,000,000 VND. Duration: Jan 2026 – Dec 2028.</div>
- <div class="grant-item">Title: An Explainable Approach Towards Trustworthy Recommender Systems. Collaborator: Singapore Management University. Source: Vietnam National University, Ho Chi Minh City (C2025-18-37). Grant: 200,000,000 VND. Duration: Oct 2025 – Mar 2027.</div>

<h3 class="home-section__header">Teaching</h3>
- <div class="teaching-item">Instructor for <strong>Data Structures and Algorithms</strong> - Faculty of Information Technology, University of Science, VNU-HCM - Spring 2026</div>
- <div class="teaching-item">Instructor for <strong>Computational Thinking</strong> - Faculty of Information Technology, University of Science, VNU-HCM - Fall 2025</div>
- <div class="teaching-item">Instructor for <strong>Fundamentals of Programming</strong> - Faculty of Information Technology, University of Science, VNU-HCM - Fall 2025</div>
- <div class="teaching-item">Teaching Assistant for <strong>CM102 - Critical Thinking</strong> - Faculty of Information Technology, University of Science, VNU-HCM - Fall 2024, Spring 2025, Fall 2025, Spring 2026</div>
- <div class="teaching-item">Teaching Assistant for <strong>SMU CS608 Recommender Systems</strong> - Master of IT in Business - Summer 2021, Summer 2022</div>
- <div class="teaching-item">Teaching Assistant for <strong>SMU CS201 Data Structures and Algorithms (BSc)</strong> - Fall 2020</div>
- <div class="teaching-item">Teaching Assistant for <strong>SMU COR-IS1702 Computational Thinking</strong> - Fall 2019, Spring 2022, Fall 2022</div>

<h3 class="home-section__header">Talks</h3>
- <div class="talk-item">2026-01-13 - Evaluation and Reproducibility of Recommendation Algorithms, at Scientific Research Club, FIT, University of Science, VNU-HCM, 2026</div>
- <div class="talk-item">2025-10-07 - Recommendation Explanations from Reviews towards Trustworthy AI, at FIT, University of Science, VNU-HCM, 2025</div>
- <div class="talk-item">2025-09-16 - Evaluative and Comparative Explanations for Recommender Systems towards Trustworthy AI, at FIT, University of Science, VNU-HCM, 2025</div>
- <div class="talk-item">2025-05-07 - Towards Trust in Recommendations: Weaving Evaluative and Comparative Explanations from Textual Data, at ATMRI, Nayang Technological University Singapore, 2025</div>
- <div class="talk-item">2024-11-13 - My recent works on recommendation explanation (3 talks) + Panel discussion: Guidedance and Experiences in Navigating Ph.D. Studies, at the 14th Scientific Conference, University of Science, VNU-HCM, 2024</div>
- <div class="talk-item">2024-07-31 - Selecting Comparative Sets of Reviews Across Multiple Items (poster), at the Singapore ACM SIGKDD Symposium 2024</div>
- <div class="talk-item">2022-07-28 - Synthesizing Aspect-Driven Recommendation Explanations from Reviews (poster), at the SDSC Industry Demo Session 2022</div>
- <div class="talk-item">2019-12-08 - Explainable Recommendation with <a href="https://github.com/PreferredAI/cornac">Cornac</a>, at the University of Science, VNU-HCM, 2019</div>

<h3 class="home-section__header">Blogs</h3>
- <div class="talk-item">2022-11-30 - <a href="https://preferred.ai/blog/recommendation-explanation">All Good Recommendations Come with an Explanation</a></div>


<h3 class="home-section__header">Projects</h3>
{% assign items = site.projects | sort: 'date' | reverse %}
{% for item in items %}
<div>
  <div>
    {{ item.title }}
  </div>
  <div>
    <small>
        <small>
            {{ item.date | date: "%Y-%m-%d" }} | 
        </small>
        <small>
            {% if item.homepage %}<a href="{{ item.homepage }}">Homepage</a>{% endif %}
        </small>
    </small>
  </div>
  <div>
    <small>
        {{ item.description }}
    </small>
  </div>
</div>
<br>
{% endfor %}