# RAD Group Newsletter Builder — Master Knowledge Base
Version: 8.0

## 1. Brand Profile & Constants
- **Company name:** RAD Group
- **Tagline:** Creating Solid Technology Foundations
- **Support email:** support@rad-group.co.uk
- **Support phone:** 0333 049 0130
- **Website:** rad-group.co.uk
- **Footer Contact String:** `support@rad-group.co.uk • 0333 049 0130 • rad-group.co.uk`
- **Logo (Do not alter):** `<img src="https://rad-group.co.uk/wp-content/uploads/2022/12/RAD-logo-white.png.webp" alt="RAD Group logo" />`

## 2. Image Library Lookup
Use ONLY these or a user-confirmed direct URL.
- **IMG-OFFICE:** Office / team photo (Alt: RAD Group team at the office)
- **IMG-ENGINEER:** Engineer providing support (Alt: RAD Group engineer providing support)
- **IMG-CABINET:** Server room / cabling (Alt: Network cabinet installed by RAD Group)

## 3. HTML Component Snippets (Mandatory Formatting)

### Section Header Container
<div class="sec-head"><span class="ico">EMOJI</span><h2>SECTION TITLE</h2><span class="rule"></span></div>

### Hot Topic Section
<section class="block">
  <div class="sec-head"><span class="ico">🔥</span><h2>Hot Topic</h2><span class="rule"></span></div>
  <div class="hot">
    <div class="accent"></div>
    <div class="body">
      <span class="tag">OWNER/TEAM</span>
      <h3>TITLE</h3>
      <p>SUMMARY</p>
    </div>
  </div>
</section>

### Team Member Feature (No Photo)
<section class="block">
  <div class="sec-head"><span class="ico">⭐</span><h2>Team Member of the Month</h2><span class="rule"></span></div>
  <div class="feature">
    <div class="who">
      <span class="tag">TEAM</span>
      <h3>NAME</h3>
      <div class="role">ROLE</div>
      <div class="team">TEAM</div>
    </div>
    <div class="detail">
      <div class="reason-label">Recognition Reason</div>
      <p class="reason">REASON</p>
      <ul class="qa">
        <li><b>Q:</b> QUESTION 1<br><b>A:</b> ANSWER 1</li>
      </ul>
    </div>
  </div>
</section>

### Standard Grid Section (Achievements / Upcoming Changes)
<section class="block">
  <div class="sec-head"><span class="ico">🏆</span><h2>SECTION TITLE</h2><span class="rule"></span></div>
  <div class="grid-2">
    <div class="card"><span class="tag">TEAM</span><h3>TITLE</h3><p>BODY</p></div>
  </div>
</section>

### Service Metrics Strip
<section class="block">
  <div class="sec-head"><span class="ico">📊</span><h2>Service Metrics</h2><span class="rule"></span></div>
  <div class="kpi-strip">
    <div class="kpi"><span class="badge">BADGE</span><div class="metric-value">VALUE</div><div class="metric-name">NAME</div><div class="metric-comment">COMMENT</div></div>
  </div>
</section>

### Customer Wins Section
<section class="block">
  <div class="sec-head"><span class="ico">🤝</span><h2>Customer Wins</h2><span class="rule"></span></div>
  <div class="card">
    <p style="margin:0 0 9px;color:var(--slate);font-size:9.7pt;">Organisations highlighted this month:</p>
    <div class="tag-row">
      <span class="tag">CLIENT 1</span>
      <span class="tag">CLIENT 2</span>
    </div>
  </div>
</section>

## 4. MASTER HTML TEMPLATE
Copy this skeleton VERBATIM. Replace the {{...}} placeholders with the formatted component snippets above. Do not alter the `<head>` section or outer containers.

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>{{NEWSLETTER_TITLE}} - {{ISSUE_MONTH}}</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/CiscoPonce/rad-newsletter-assets@main/style.css">
</head>
<body>
<button class="print-button" onclick="window.print()">⤓ Download PDF</button>

<div class="page">
  <div class="topbar">
    <div class="brand">
      <img src="https://rad-group.co.uk/wp-content/uploads/2022/12/RAD-logo-white.png.webp" alt="RAD Group logo" />
      <span class="wordmark">RAD Group</span>
    </div>
    <div class="edition"><b>{{ISSUE_LABEL_SHORT}}</b></div>
  </div>

  <header class="hero">
    <span class="eyebrow">{{EYEBROW}}</span>
    <h1>{{HERO_HEADLINE}}</h1>
    <p>{{HERO_SUBLINE}}</p>
  </header>

  {{HOT_TOPIC_SECTION}}
  {{TEAM_FEATURE_SECTION}}
  {{ACHIEVEMENTS_SECTION}}
  {{METRICS_SECTION}}
  {{KB_SECURITY_SECTION}}
  {{UPCOMING_CHANGES_SECTION}}
  {{CERTS_TICKET_SECTION}}
  {{CUSTOMER_WINS_SECTION}}
  {{LOOKING_AHEAD_SECTION}}
  {{SPECIAL_MENTIONS_SECTION}}

  <footer class="footer">
    <div class="f-left">
      <strong>RAD Group</strong> &nbsp; {{TAGLINE}}<br>
      {{FOOTER_CONTACT}}
    </div>
    <div class="f-right">
      <span>{{ISSUE_LABEL}}</span>
      {{FOOTER_STATUS}}
    </div>
  </footer>
</div>
</body>
</html>
```