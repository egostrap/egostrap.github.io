/**
 * EgoStrap Global Interactive Script
 * Provides premium UI features, mockup controls, card mouse-glow tracking,
 * and live statistic simulations.
 */

document.addEventListener('DOMContentLoaded', () => {
  setupMobileMenu();
  setupNavbarActiveState();
  setupLauncherMockup();
  setupMouseGlowCards();
  simulateStats();
});

/**
 * Mobile Navigation Drawer Toggle
 */
function setupMobileMenu() {
  const toggleBtn = document.querySelector('.menu-toggle');
  const navLinks = document.querySelector('.nav-links');

  if (toggleBtn && navLinks) {
    toggleBtn.addEventListener('click', (e) => {
      e.stopPropagation();
      navLinks.classList.toggle('active');
      const isExpanded = navLinks.classList.contains('active');
      toggleBtn.innerHTML = isExpanded ? '✕' : '☰';
    });

    // Close menu when clicking outside
    document.addEventListener('click', (e) => {
      if (!navLinks.contains(e.target) && !toggleBtn.contains(e.target)) {
        navLinks.classList.remove('active');
        toggleBtn.innerHTML = '☰';
      }
    });
  }
}

/**
 * Highlights active page in the header links
 */
function setupNavbarActiveState() {
  const currentPath = window.location.pathname;
  const navLinks = document.querySelectorAll('.nav-links a');
  
  navLinks.forEach(link => {
    const href = link.getAttribute('href');
    if (href && currentPath.includes(href) && href !== 'index.html') {
      link.classList.add('active');
    } else if (href === 'index.html' && (currentPath.endsWith('/') || currentPath.endsWith('index.html'))) {
      link.classList.add('active');
    }
  });
}

/**
 * Launcher Dashboard Mockup Interactivity
 */
function setupLauncherMockup() {
  const sidebarItems = document.querySelectorAll('.launcher-sidebar .sidebar-item');
  const views = document.querySelectorAll('.launcher-content .launcher-view');
  const launchBtn = document.querySelector('.btn-launch');
  const launchStatus = document.querySelector('.launch-status');

  sidebarItems.forEach(item => {
    item.addEventListener('click', () => {
      const targetViewId = item.getAttribute('data-view');
      const targetView = document.getElementById(`view-${targetViewId}`);

      if (targetView) {
        // Toggle Active Sidebar Link
        sidebarItems.forEach(si => si.classList.remove('active'));
        item.classList.add('active');

        // Toggle Active Content View
        views.forEach(v => v.classList.remove('active'));
        targetView.classList.add('active');
      }
    });
  });

  // Action simulation for "Launch Roblox" button
  if (launchBtn && launchStatus) {
    let launching = false;
    launchBtn.addEventListener('click', () => {
      if (launching) return;
      launching = true;
      
      launchBtn.style.opacity = '0.7';
      launchBtn.innerText = 'Booting...';
      
      const originalStatusText = launchStatus.innerHTML;
      launchStatus.innerHTML = '<span class="badge-dot" style="background:#ffb700;"></span> Running Client-side patches...';

      setTimeout(() => {
        launchStatus.innerHTML = '<span class="badge-dot" style="background:#10b981;"></span> Launching Roblox Player...';
      }, 1200);

      setTimeout(() => {
        launchStatus.innerHTML = '<span class="badge-dot" style="background:#00d2ff;"></span> EgoStrap Hooked successfully!';
        launchBtn.style.opacity = '1';
        launchBtn.innerText = 'Active';
        
        // Reset after 3 seconds
        setTimeout(() => {
          launchStatus.innerHTML = originalStatusText;
          launchBtn.innerText = 'Launch';
          launching = false;
        }, 3000);
      }, 2500);
    });
  }
}

/**
 * Futuristic card border mouse-glow effect tracker (updates relative coordinates)
 */
function setupMouseGlowCards() {
  const cards = document.querySelectorAll('.feature-card, .donate-card, .timeline-content');
  
  cards.forEach(card => {
    card.addEventListener('mousemove', (e) => {
      const rect = card.getBoundingClientRect();
      const x = e.clientX - rect.left;
      const y = e.clientY - rect.top;
      
      card.style.setProperty('--x', `${x}px`);
      card.style.setProperty('--y', `${y}px`);
    });
  });
}

/**
 * Dynamic statistics counters for simulated usage activity
 */
function simulateStats() {
  const downloadCount = document.getElementById('stat-dl-count');
  const onlineCount = document.getElementById('stat-online-count');

  // Base starting counts matching official stats
  let dlNum = 245987;
  let onlineNum = 14203;

  if (downloadCount) downloadCount.innerText = dlNum.toLocaleString();
  if (onlineCount) onlineCount.innerText = onlineNum.toLocaleString();

  // Periodically increment stats dynamically to simulate active website usage
  setInterval(() => {
    if (downloadCount && Math.random() > 0.3) {
      dlNum += Math.floor(Math.random() * 3) + 1;
      downloadCount.innerText = dlNum.toLocaleString();
    }
    
    if (onlineCount) {
      const change = Math.floor(Math.random() * 11) - 5; // -5 to +5 change
      onlineNum += change;
      onlineCount.innerText = onlineNum.toLocaleString();
    }
  }, 4000);
}
