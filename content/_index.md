---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'News'
      subtitle: ''
      text: |-
          <div class="space-y-2 text-sm">
            <!-- 2025 entries -->
            <div class="flex">
              <strong class="w-24">6.2025</strong>
              <span>📄 Accepted paper in ISMIR 2025, Daejeon, South Korea</span>
            </div>
            <div class="flex">
              <strong class="w-24">5.2025</strong>
              <span>🎓 Accepted as Lecturer at Higher Colleges of Technology (oldest uni in UAE)</span>
            </div>
            <div class="flex">
              <strong class="w-24">5.2025</strong>
              <span>🎉 Graduated from MS in Machine Learning, MBZUAI</span>
            </div>

            <!-- 2023–2020 entries -->
            <div class="flex">
              <strong class="w-24">2023</strong>
              <span>🎓 Awarded full scholarship for MS in Machine Learning at MBZUAI</span>
            </div>
            <div class="flex">
              <strong class="w-24">2023</strong>
              <span>💼 Data Scientist at Advance.AI, Singapore &amp; Jakarta</span>
            </div>
            <div class="flex">
              <strong class="w-24">2022</strong>
              <span>🚀 Built first startup “Reviewein” and led a team of 10+ members</span>
            </div>
            <div class="flex">
              <strong class="w-24">2022</strong>
              <span>💡 Awarded Stanford Innovation Fellowship</span>
            </div>
            <div class="flex">
              <strong class="w-24">2021</strong>
              <span>🏅 Awarded “Most Outstanding Student,” School of Computer Science, University of Indonesia</span>
            </div>
            <div class="flex">
              <strong class="w-24">2020</strong>
              <span>🌍 Awarded Erasmus+ Scholarship</span>
            </div>
          </div>
      # text: |-
      #   **June 2025**	📄 Accepted paper in ISMIR 2025, Daejeon, South Korea
      #   **May 2025**	🎓 Accepted as Lecturer in Higher Colleges of Technology (oldest uni in UAE)
      #   **May 2025**	🎉 Graduated from MS Machine Learning, MBZUAI

    design:
      columns: '1'

  # - block: html
  #   content: |-
  #     <div class="space-y-2 text-sm">
  #       <!-- 2025 entries -->
  #       <div class="flex">
  #         <strong class="w-24">June 2025</strong>
  #         <span>📄 Accepted paper in ISMIR 2025, Daejeon, South Korea</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">May 2025</strong>
  #         <span>🎓 Accepted as Lecturer at Higher Colleges of Technology (oldest uni in UAE)</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">May 2025</strong>
  #         <span>🎉 Graduated from MS in Machine Learning, MBZUAI</span>
  #       </div>

  #       <!-- 2023–2020 entries -->
  #       <div class="flex">
  #         <strong class="w-24">2023</strong>
  #         <span>🎓 Awarded full scholarship for MS in Machine Learning at MBZUAI</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">2022</strong>
  #         <span>🚀 Built first startup “Reviewein” and led a team of 10+ members</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">2022</strong>
  #         <span>💡 Awarded Stanford Innovation Fellowship</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">2021</strong>
  #         <span>🏅 Awarded “Most Outstanding Student,” School of Computer Science, University of Indonesia</span>
  #       </div>
  #       <div class="flex">
  #         <strong class="w-24">2020</strong>
  #         <span>🌍 Awarded Erasmus+ Scholarship</span>
  #       </div>
  #     </div>
  #   design:
  #     columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 4
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
