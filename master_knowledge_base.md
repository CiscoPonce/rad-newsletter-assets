# RAD Group Newsletter Builder — Master Knowledge Base
Version: 8.0

## 1. Brand Profile & Constants
- **Company name:** RAD Group
- **Tagline:** Creating Solid Technology Foundations
- **Support email:** support@rad-group.co.uk
- **Support phone:** 0333 049 0130
- **Website:** rad-group.co.uk
- **Footer Contact String:** `support@rad-group.co.uk • 0333 049 0130 • rad-group.co.uk`

## 2. Image Library Lookup
Use ONLY these or a user-confirmed direct URL.
- **IMG-OFFICE:** Office / team photo (Alt: RAD Group team at the office)
- **IMG-ENGINEER:** Engineer providing support (Alt: RAD Group engineer providing support)
- **IMG-CABINET:** Server room / cabling (Alt: Network cabinet installed by RAD Group)

## 3. HTML Component Snippets (Mandatory Formatting)
Substitute the content gathered from the user into these exact structural blocks. 

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