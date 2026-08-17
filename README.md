<style>
  .header-container {
    width: 100%;
    padding: 3rem 2rem;
    text-align: center;
    background: linear-gradient(135deg, #f8f7f4 0%, #ffffff 100%);
    border-radius: 12px;
    border: 1px solid #e5e5e5;
  }
  
  .greeting-emoji {
    display: inline-block;
    font-size: 2.5rem;
    margin-bottom: 1rem;
    animation: wave 1.5s ease-in-out infinite;
    transform-origin: 70% 70%;
  }
  
  @keyframes wave {
    0%, 100% { transform: rotate(0deg); }
    25% { transform: rotate(14deg); }
    75% { transform: rotate(-8deg); }
  }
  
  .name-main {
    font-size: 2.8rem;
    font-weight: 500;
    color: #0b0b0b;
    margin: 0.5rem 0;
    letter-spacing: -0.5px;
    animation: slideDown 0.8s ease-out;
  }
  
  @keyframes slideDown {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  .title-accent {
    position: relative;
    font-size: 1.3rem;
    color: #185FA5;
    margin: 1rem 0 0 0;
    font-weight: 500;
    animation: slideUp 0.8s ease-out 0.2s backwards;
  }
  
  .title-accent::after {
    content: '';
    position: absolute;
    bottom: -8px;
    left: 50%;
    transform: translateX(-50%);
    width: 0;
    height: 2px;
    background: #378ADD;
    border-radius: 1px;
    animation: expandWidth 0.6s ease-out 0.6s forwards;
  }
  
  @keyframes slideUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  @keyframes expandWidth {
    from { width: 0; }
    to { width: 100%; }
  }
  
  .description {
    font-size: 1rem;
    color: #666;
    line-height: 1.6;
    margin: 2rem auto 0;
    max-width: 580px;
    animation: fadeIn 0.8s ease-out 0.4s backwards;
  }
  
  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }
  
  .stats-container {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin-top: 2.5rem;
    flex-wrap: wrap;
    animation: fadeIn 0.8s ease-out 0.6s backwards;
  }
  
  .stat-item {
    text-align: center;
    padding: 0.75rem 1.5rem;
    border-radius: 8px;
    background: #f5f5f5;
    border: 1px solid #e5e5e5;
    cursor: pointer;
    transition: all 0.3s ease;
    min-width: 120px;
  }
  
  .stat-item:hover {
    border-color: #ccc;
    background: #efefef;
    transform: translateY(-3px);
  }
  
  .stat-value {
    font-size: 1.5rem;
    font-weight: 500;
    color: #378ADD;
    display: block;
  }
  
  .stat-label {
    font-size: 0.85rem;
    color: #666;
    margin-top: 0.25rem;
  }
  
  .divider {
    height: 1px;
    background: #e5e5e5;
    margin: 2rem auto;
    width: 80px;
    animation: expandWidth 0.8s ease-out 0.8s backwards;
  }
  
  @media (max-width: 600px) {
    .header-container { padding: 2rem 1.5rem; }
    .name-main { font-size: 2rem; }
    .title-accent { font-size: 1.1rem; }
    .stats-container { gap: 1rem; }
    .stat-item { min-width: 100px; padding: 0.6rem 1rem; }
  }
</style>

<div class="header-container">
  <div class="greeting-emoji">👋</div>
  <h1 class="name-main">Hi, I'm Yuan Gonzalez</h1>
  <div class="divider"></div>
  <h2 class="title-accent">Data Analyst & Business Intelligence Enthusiast</h2>
  <p class="description">
    Transforming raw data into actionable insights through intuitive dashboards, advanced analytics, and intelligent business solutions.
  </p>
  <div class="stats-container">
    <div class="stat-item">
      <span class="stat-value">📊</span>
      <span class="stat-label">Analytics</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">💾</span>
      <span class="stat-label">SQL Expert</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">📈</span>
      <span class="stat-label">Power BI</span>
    </div>
    <div class="stat-item">
      <span class="stat-value">🐍</span>
      <span class="stat-label">Python</span>
    </div>
  </div>
</div>
