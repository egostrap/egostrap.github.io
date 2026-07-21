/**
 * EgoStrap Docs Navigation & Search Script
 * Handles category navigation, content loading and article search filters.
 */

document.addEventListener('DOMContentLoaded', () => {
  setupDocsNavigation();
  setupDocsSearch();
});

/**
 * Handles tab-like routing inside the documentation page
 */
function setupDocsNavigation() {
  const sidebarLinks = document.querySelectorAll('.docs-link');
  const sections = document.querySelectorAll('.docs-section');

  // Check URL hash for direct links (e.g. docs.html#installation)
  const currentHash = window.location.hash;
  if (currentHash) {
    const targetId = currentHash.replace('#', '');
    const activeSection = document.getElementById(targetId);
    const activeLink = document.querySelector(`.docs-link[data-target="${targetId}"]`);
    
    if (activeSection && activeLink) {
      sections.forEach(s => s.classList.remove('active'));
      activeSection.classList.add('active');
      
      sidebarLinks.forEach(l => l.classList.remove('active'));
      activeLink.classList.add('active');
    }
  }

  sidebarLinks.forEach(link => {
    link.addEventListener('click', (e) => {
      e.preventDefault();
      const targetId = link.getAttribute('data-target');
      const targetSection = document.getElementById(targetId);

      if (targetSection) {
        // Update URL hash without reload
        window.location.hash = targetId;

        // Toggle Sidebar classes
        sidebarLinks.forEach(l => l.classList.remove('active'));
        link.classList.add('active');

        // Switch active section content
        sections.forEach(s => s.classList.remove('active'));
        targetSection.classList.add('active');

        // Scroll to top of docs content on mobile
        if (window.innerWidth <= 768) {
          targetSection.scrollIntoView({ behavior: 'smooth' });
        } else {
          window.scrollTo({ top: 0, behavior: 'smooth' });
        }
      }
    });
  });
}

/**
 * Filters sidebar navigation links based on doc search string
 */
function setupDocsSearch() {
  const searchInput = document.querySelector('.docs-search');
  const sidebarLinks = document.querySelectorAll('.docs-link');
  const groups = document.querySelectorAll('.docs-menu > div'); // Nav category wrappers

  if (!searchInput) return;

  searchInput.addEventListener('input', (e) => {
    const query = e.target.value.toLowerCase().trim();

    sidebarLinks.forEach(link => {
      const text = link.textContent.toLowerCase();
      const targetId = link.getAttribute('data-target');
      const section = document.getElementById(targetId);
      
      // Look inside both the link label and the actual section text content
      const contentText = section ? section.textContent.toLowerCase() : '';
      
      if (text.includes(query) || contentText.includes(query)) {
        link.style.display = 'block';
      } else {
        link.style.display = 'none';
      }
    });

    // Hide entire categories if all of their children links are hidden
    groups.forEach(group => {
      const visibleLinks = group.querySelectorAll('.docs-link[style="display: block;"], .docs-link:not([style*="display: none"])');
      const categoryTitle = group.querySelector('.docs-cat-title');
      
      if (visibleLinks.length === 0) {
        group.style.display = 'none';
      } else {
        group.style.display = 'block';
      }
    });
  });
}
