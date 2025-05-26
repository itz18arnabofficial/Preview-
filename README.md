<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EduNeon - Smart Learning Platform</title>
<script src="https://cdn.tailwindcss.com"></script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/remixicon@4.5.0/fonts/remixicon.css" rel="stylesheet"/>
<script>
tailwind.config = {
theme: {
extend: {
colors: {
primary: '#6366f1',
secondary: '#0ea5e9'
},
borderRadius: {
'none': '0px',
'sm': '4px',
DEFAULT: '8px',
'md': '12px',
'lg': '16px',
'xl': '20px',
'2xl': '24px',
'3xl': '32px',
'full': '9999px',
'button': '8px'
}
}
}
}
</script>
<style>
:where([class^="ri-"])::before { content: "\f3c2"; }
.neon-glow { box-shadow: 0 0 15px rgba(99, 102, 241, 0.2); }
.board-card:hover { transform: translateY(-5px); }
.chapter-list { max-height: 0; overflow: hidden; transition: max-height 0.3s ease-out; }
.chapter-list.active { max-height: 1000px; }
.class-filter.active { background-color: #6366f1 !important; color: white !important; }
</style>
</head>
<body class="bg-white min-h-screen">
<header class="fixed w-full bg-white/90 backdrop-blur-sm z-50 border-b">
<nav class="container mx-auto px-6 py-4 flex items-center justify-between">
<a href="#" class="text-2xl font-['Pacifico'] text-primary">logo</a>
<div class="flex items-center gap-8">
<a href="#" class="text-gray-700 hover:text-primary transition-colors">Home</a>
<a href="#boards" class="text-gray-700 hover:text-primary transition-colors">Boards</a>
<a href="#about" class="text-gray-700 hover:text-primary transition-colors">About</a>
<button class="w-10 h-10 flex items-center justify-center text-gray-700 hover:text-primary transition-colors">
<i class="ri-more-2-fill ri-xl"></i>
</button>
</div>
</nav>
</header>
<main>
<section class="pt-24 pb-20 relative overflow-hidden">
<div class="absolute inset-0 bg-[url('https://public.readdy.ai/ai/img_res/96c277f5784dbc4a1f23a3d6485f271c.jpg')] bg-cover bg-center opacity-10"></div>
<div class="container mx-auto px-6 relative">
<div class="max-w-3xl">
<h1 class="text-5xl font-bold text-gray-900 mb-6">Transform Your Learning Journey with Smart Education</h1>
<p class="text-xl text-gray-600 mb-10">Access comprehensive study materials across CBSE, WBBSE, and ICSE boards. Enhanced learning experience with AI-powered resources and expert-curated content.</p>
<a href="#boards" class="inline-flex items-center px-6 py-3 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90 transition-colors" onclick="document.querySelector('#boards').scrollIntoView({behavior: 'smooth', block: 'start'})">
Explore Boards
<i class="ri-arrow-right-line ml-2"></i>
</a>
</div>
</div>
</section>
<section id="boards" class="py-20 bg-gray-50">
<div class="container mx-auto px-6">
<h2 class="text-3xl font-bold text-center text-gray-900 mb-4">Choose Your Board</h2>
<p class="text-gray-600 text-center mb-12 max-w-2xl mx-auto">Select from our comprehensive collection of study materials tailored for different educational boards.</p>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="board-card bg-white rounded-lg p-6 neon-glow transition-all duration-300 cursor-pointer">
<div class="h-48 mb-6 rounded-lg overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/e526d8ce2c667a8b72aba8f683ac3568.jpg"
class="w-full h-full object-cover" alt="CBSE">
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">CBSE Board</h3>
<p class="text-gray-600">Comprehensive study materials aligned with CBSE curriculum standards.</p>
</div>
<div class="board-card bg-white rounded-lg p-6 neon-glow transition-all duration-300 cursor-pointer">
<div class="h-48 mb-6 rounded-lg overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/5fa1566adcdea8b5e4843ca3d9ccd92e.jpg"
class="w-full h-full object-cover" alt="WBBSE">
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">WBBSE Board</h3>
<p class="text-gray-600">Expert-curated content following WBBSE guidelines and patterns.</p>
</div>
<div class="board-card bg-white rounded-lg p-6 neon-glow transition-all duration-300 cursor-pointer">
<div class="h-48 mb-6 rounded-lg overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/90a1820f9a803e8e178e7a542640345c.jpg"
class="w-full h-full object-cover" alt="ICSE">
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">ICSE Board</h3>
<p class="text-gray-600">Quality study materials designed specifically for ICSE students.</p>
</div>
</div>
<div class="mt-16 bg-white rounded-lg p-8 neon-glow">
<h3 class="text-2xl font-bold text-gray-900 mb-6 text-center">Upcoming Examinations</h3>
<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
<div class="p-6 bg-gray-50 rounded-lg">
<div class="flex items-center justify-between mb-4">
<h4 class="text-lg font-semibold text-gray-900">CBSE Board Exam 2025</h4>
<span class="px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full">March 2025</span>
</div>
<p class="text-gray-600 mb-4">Class 10 & 12 Board Examinations</p>
<button class="w-full px-4 py-2 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90 transition-colors">View Schedule</button>
</div>
<div class="p-6 bg-gray-50 rounded-lg">
<div class="flex items-center justify-between mb-4">
<h4 class="text-lg font-semibold text-gray-900">WBBSE Madhyamik 2025</h4>
<span class="px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full">February 2025</span>
</div>
<p class="text-gray-600 mb-4">Class 10 Board Examinations</p>
<button class="w-full px-4 py-2 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90 transition-colors">View Schedule</button>
</div>
<div class="p-6 bg-gray-50 rounded-lg">
<div class="flex items-center justify-between mb-4">
<h4 class="text-lg font-semibold text-gray-900">ICSE & ISC 2025</h4>
<span class="px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full">April 2025</span>
</div>
<p class="text-gray-600 mb-4">Class 10 & 12 Board Examinations</p>
<button class="w-full px-4 py-2 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90 transition-colors">View Schedule</button>
</div>
</div>
</div>
</div>
</section>
<section id="features" class="py-20">
<div class="container mx-auto px-6">
<div class="bg-white rounded-lg p-8 neon-glow mb-12">
<h3 class="text-2xl font-bold text-gray-900 mb-6 text-center">Exam Preparation Tips</h3>
<div class="grid grid-cols-1 md:grid-cols-4 gap-6">
<div class="p-4">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-time-line text-primary ri-xl"></i>
</div>
<h4 class="text-lg font-semibold text-gray-900 mb-2">Time Management</h4>
<p class="text-gray-600">Create a study schedule and stick to it. Allocate time based on subject difficulty.</p>
</div>
<div class="p-4">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-file-list-3-line text-primary ri-xl"></i>
</div>
<h4 class="text-lg font-semibold text-gray-900 mb-2">Practice Papers</h4>
<p class="text-gray-600">Solve previous years' question papers and take mock tests regularly.</p>
</div>
<div class="p-4">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-mind-map text-primary ri-xl"></i>
</div>
<h4 class="text-lg font-semibold text-gray-900 mb-2">Mind Mapping</h4>
<p class="text-gray-600">Use mind maps and flowcharts to understand and remember complex topics.</p>
</div>
<div class="p-4">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-rest-time-line text-primary ri-xl"></i>
</div>
<h4 class="text-lg font-semibold text-gray-900 mb-2">Regular Breaks</h4>
<p class="text-gray-600">Take short breaks between study sessions to maintain focus and productivity.</p>
</div>
</div>
</div>
<div class="container mx-auto px-6">
<h2 class="text-3xl font-bold text-center text-gray-900 mb-4">Why Choose Us</h2>
<p class="text-gray-600 text-center mb-12 max-w-2xl mx-auto">Experience the perfect blend of traditional learning and modern technology.</p>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="p-6 bg-white rounded-lg neon-glow">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-book-line text-primary ri-xl"></i>
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">Comprehensive Content</h3>
<p class="text-gray-600">Access detailed study materials, practice questions, and previous year papers.</p>
</div>
<div class="p-6 bg-white rounded-lg neon-glow">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-ai-generate text-primary ri-xl"></i>
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">AI-Powered Learning</h3>
<p class="text-gray-600">Personalized learning paths and adaptive assessments for better results.</p>
</div>
<div class="p-6 bg-white rounded-lg neon-glow">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-24-hours-line text-primary ri-xl"></i>
</div>
<h3 class="text-xl font-bold text-gray-900 mb-2">24/7 Accessibility</h3>
<p class="text-gray-600">Study anytime, anywhere with our digital platform and downloadable resources.</p>
</div>
</div>
</div>
</section>
</main>
<footer class="bg-gray-50 py-12">
<div class="container mx-auto px-6">
<div class="grid grid-cols-1 md:grid-cols-4 gap-8">
<div>
<a href="#" class="text-2xl font-['Pacifico'] text-primary block mb-4">logo</a>
<p class="text-gray-600">Empowering students with smart learning solutions.</p>
</div>
<div>
<h4 class="font-bold text-gray-900 mb-4">Quick Links</h4>
<ul class="space-y-2">
<li><a href="#" class="text-gray-600 hover:text-primary">Home</a></li>
<li><a href="#boards" class="text-gray-600 hover:text-primary">Boards</a></li>
<li><a href="#about" class="text-gray-600 hover:text-primary">About Us</a></li>
</ul>
</div>
<div>
<h4 class="font-bold text-gray-900 mb-4">Contact</h4>
<ul class="space-y-2">
<li class="text-gray-600">support@eduneon.com</li>
<li class="text-gray-600">+1 (555) 123-4567</li>
</ul>
</div>
<div>
<h4 class="font-bold text-gray-900 mb-4">Follow Us</h4>
<div class="flex space-x-4">
<a href="#" class="w-10 h-10 flex items-center justify-center text-gray-600 hover:text-primary">
<i class="ri-facebook-fill ri-lg"></i>
</a>
<a href="#" class="w-10 h-10 flex items-center justify-center text-gray-600 hover:text-primary">
<i class="ri-twitter-fill ri-lg"></i>
</a>
<a href="#" class="w-10 h-10 flex items-center justify-center text-gray-600 hover:text-primary">
<i class="ri-instagram-fill ri-lg"></i>
</a>
</div>
</div>
</div>
<div class="border-t border-gray-200 mt-12 pt-8 text-center text-gray-600">
<p>&copy; 2025 EduNeon. All rights reserved.</p>
</div>
</div>
</footer>
<div id="subjectModal" class="fixed inset-0 bg-black/50 hidden items-center justify-center z-50">
<div class="bg-white rounded-lg w-full max-w-4xl mx-4 p-6 max-h-[90vh] overflow-y-auto">
<div class="flex justify-between items-center mb-6">
<h3 class="text-2xl font-bold text-gray-900" id="modalTitle">CBSE Board Subjects</h3>
<button class="w-10 h-10 flex items-center justify-center text-gray-500 hover:text-gray-700" onclick="closeSubjectModal()">
<i class="ri-close-line ri-xl"></i>
</button>
</div>
<div class="mb-6">
<div class="flex items-center justify-between mb-4">
<h4 class="text-xl font-semibold text-gray-900">Select Class</h4>
<div class="flex gap-2">
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter active" data-class="all">All Classes</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="6">Class 6</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="7">Class 7</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="8">Class 8</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="9">Class 9</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="10">Class 10</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="11">Class 11</button>
<button class="px-4 py-2 text-sm font-medium text-gray-700 bg-gray-100 hover:bg-gray-200 !rounded-button class-filter" data-class="12">Class 12</button>
</div>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer" data-class="6,7,8,9,10,11,12">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-book-2-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">Bengali</h4>
<p class="text-gray-600 mb-4">Literature, Grammar and Communication</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-book-open-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">English</h4>
<p class="text-gray-600 mb-4">Literature, Grammar and Communication</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-numbers-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">Mathematics</h4>
<p class="text-gray-600 mb-4">Algebra, Geometry and Statistics</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-flask-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">Physical Science</h4>
<p class="text-gray-600 mb-4">Physics and Chemistry</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-seedling-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">Life Science</h4>
<p class="text-gray-600 mb-4">Biology and Environmental Science</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-ancient-gate-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">History</h4>
<p class="text-gray-600 mb-4">Indian and World History</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="ri-global-line text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">Geography</h4>
<p class="text-gray-600 mb-4">Physical and Human Geography</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">5 Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
</div>
</div>
</div>
<script>
const boardTitles = {
'CBSE Board': 'CBSE Board Subjects',
'WBBSE Board': 'WBBSE Board Subjects',
'ICSE Board': 'ICSE Board Subjects'
};
document.querySelectorAll('.class-filter').forEach(button => {
button.addEventListener('click', () => {
document.querySelectorAll('.class-filter').forEach(btn => btn.classList.remove('active', 'bg-primary', 'text-white'));
button.classList.add('active', 'bg-primary', 'text-white');
const selectedClass = button.dataset.class;
document.querySelectorAll('.subject-card').forEach(card => {
const classes = card.dataset.class.split(',');
if (selectedClass === 'all' || classes.includes(selectedClass)) {
card.style.display = 'block';
} else {
card.style.display = 'none';
}
});
});
});
const subjectsByBoard = {
'ICSE Board': [
{
name: 'English',
icon: 'ri-book-open-line',
description: 'Literature, Grammar and Communication',
chapters: 5
},
{
name: 'Bengali/Hindi/Others',
icon: 'ri-translate-2-line',
description: 'Second Language Studies',
chapters: 5
},
{
name: 'Mathematics',
icon: 'ri-numbers-line',
description: 'Algebra, Geometry and Statistics',
chapters: 5
},
{
name: 'Physics',
icon: 'ri-rocket-line',
description: 'Mechanics, Energy and Modern Physics',
chapters: 5
},
{
name: 'Chemistry',
icon: 'ri-flask-line',
description: 'Organic and Inorganic Chemistry',
chapters: 5
},
{
name: 'Biology',
icon: 'ri-seedling-line',
description: 'Life Sciences and Human Biology',
chapters: 5
},
{
name: 'History and Civics',
icon: 'ri-ancient-gate-line',
description: 'Indian History and Civic Studies',
chapters: 5
},
{
name: 'Geography',
icon: 'ri-global-line',
description: 'Physical and Human Geography',
chapters: 5
}
]
};
document.querySelectorAll('.board-card').forEach(card => {
card.addEventListener('click', () => {
const boardTitle = card.querySelector('h3').textContent;
document.getElementById('modalTitle').textContent = boardTitles[boardTitle];
const subjectGrid = document.querySelector('#subjectModal .grid');
if(boardTitle === 'ICSE Board') {
subjectGrid.innerHTML = subjectsByBoard[boardTitle].map(subject => `
<div class="subject-card bg-white border rounded-lg p-6 hover:shadow-lg transition-shadow cursor-pointer">
<div class="w-12 h-12 flex items-center justify-center bg-primary/10 rounded-full mb-4">
<i class="${subject.icon} text-primary ri-xl"></i>
</div>
<h4 class="text-xl font-semibold text-gray-900 mb-2">${subject.name}</h4>
<p class="text-gray-600 mb-4">${subject.description}</p>
<div class="flex justify-between items-center">
<span class="text-sm text-gray-500">${subject.chapters} Chapters</span>
<i class="ri-arrow-right-line text-primary"></i>
</div>
</div>
`).join('');
}
document.getElementById('subjectModal').classList.remove('hidden');
document.getElementById('subjectModal').classList.add('flex');
document.body.style.overflow = 'hidden';
});
});
function closeSubjectModal() {
document.getElementById('subjectModal').classList.add('hidden');
document.getElementById('subjectModal').classList.remove('flex');
document.body.style.overflow = 'auto';
}
document.querySelectorAll('.subject-card').forEach(card => {
card.addEventListener('click', () => {
const subjectName = card.querySelector('h4').textContent;
showChapterModal(subjectName);
});
});
function showChapterModal(subjectName) {
const chapterData = {
'English': [
{title: 'First Flight (Prose)', duration: '4 hours', progress: 70},
{title: 'Footprints Without Feet', duration: '3.5 hours', progress: 45},
{title: 'Grammar & Writing', duration: '5 hours', progress: 85},
{title: 'Literature Reader', duration: '4 hours', progress: 25},
{title: 'Reading Comprehension', duration: '3 hours', progress: 60},
],
'Bengali/Hindi/Others': [
{title: 'Literature', duration: '3 hours', progress: 65},
{title: 'Grammar', duration: '3.5 hours', progress: 40},
{title: 'Writing', duration: '3 hours', progress: 75},
{title: 'Reading', duration: '2.5 hours', progress: 30},
{title: 'Communication', duration: '3 hours', progress: 55},
],
'Mathematics': [
{title: 'Real Numbers', duration: '4 hours', progress: 70},
{title: 'Polynomials & Quadratic Equations', duration: '5 hours', progress: 45},
{title: 'Coordinate Geometry', duration: '4 hours', progress: 85},
{title: 'Trigonometry & Applications', duration: '5 hours', progress: 25},
{title: 'Statistics & Probability', duration: '4 hours', progress: 60},
],
'Physics': [
{title: 'Mechanics', duration: '3 hours', progress: 75},
{title: 'Heat and Energy', duration: '3.5 hours', progress: 50},
{title: 'Light and Sound', duration: '3 hours', progress: 65},
{title: 'Electricity', duration: '3 hours', progress: 40},
{title: 'Modern Physics', duration: '2.5 hours', progress: 80},
],
'Chemistry': [
{title: 'Atomic Structure', duration: '3 hours', progress: 70},
{title: 'Chemical Bonding', duration: '3.5 hours', progress: 45},
{title: 'Organic Chemistry', duration: '3 hours', progress: 85},
{title: 'Physical Chemistry', duration: '2.5 hours', progress: 25},
{title: 'Periodic Table', duration: '3 hours', progress: 60},
],
'Biology': [
{title: 'Cell Biology', duration: '3 hours', progress: 65},
{title: 'Human Physiology', duration: '3.5 hours', progress: 40},
{title: 'Plant Biology', duration: '3 hours', progress: 75},
{title: 'Genetics', duration: '2.5 hours', progress: 30},
{title: 'Ecology', duration: '3 hours', progress: 55},
],
'History and Civics': [
{title: 'Ancient India', duration: '3 hours', progress: 70},
{title: 'Medieval India', duration: '3.5 hours', progress: 45},
{title: 'Modern India', duration: '3 hours', progress: 85},
{title: 'World History', duration: '2.5 hours', progress: 25},
{title: 'Civics', duration: '3 hours', progress: 60},
],
'Geography': [
{title: 'Physical Geography', duration: '3 hours', progress: 65},
{title: 'Climate', duration: '3.5 hours', progress: 40},
{title: 'Resources', duration: '3 hours', progress: 75},
{title: 'Population', duration: '2.5 hours', progress: 30},
{title: 'Map Work', duration: '3 hours', progress: 55},
],
'English': [
{title: 'Reading Comprehension', duration: '3 hours', progress: 75},
{title: 'Writing and Grammar', duration: '3.5 hours', progress: 60},
{title: 'Literature Reader', duration: '2.5 hours', progress: 40},
{title: 'Communication Skills', duration: '3 hours', progress: 85},
{title: 'Vocabulary Building', duration: '4 hours', progress: 30},
],
'Mathematics': [
{title: 'Number Systems', duration: '3 hours', progress: 65},
{title: 'Algebra', duration: '3.5 hours', progress: 45},
{title: 'Geometry', duration: '3 hours', progress: 80},
{title: 'Mensuration', duration: '3 hours', progress: 20},
{title: 'Statistics', duration: '2.5 hours', progress: 90},
],
'Physical Science': [
{title: 'Chemical Reactions & Equations', duration: '4 hours', progress: 70},
{title: 'Acids, Bases & Salts', duration: '3.5 hours', progress: 55},
{title: 'Light - Reflection & Refraction', duration: '4 hours', progress: 35},
{title: 'Electricity & Magnetic Effects', duration: '5 hours', progress: 80},
{title: 'Sources of Energy', duration: '3 hours', progress: 25},
],
'Life Science': [
{title: 'Life Processes', duration: '4 hours', progress: 60},
{title: 'Control & Coordination', duration: '3.5 hours', progress: 40},
{title: 'Reproduction in Organisms', duration: '4 hours', progress: 75},
{title: 'Heredity & Evolution', duration: '4.5 hours', progress: 30},
{title: 'Our Environment', duration: '3 hours', progress: 85},
],
'History': [
{title: 'Rise of Nationalism in Europe', duration: '4 hours', progress: 65},
{title: 'Nationalism in India', duration: '4.5 hours', progress: 40},
{title: 'Making of Global World', duration: '4 hours', progress: 75},
{title: 'Print Culture & Modern World', duration: '3.5 hours', progress: 30},
{title: 'Democratic Politics', duration: '4 hours', progress: 20},
],
'Geography': [
{title: 'Resources & Development', duration: '4 hours', progress: 70},
{title: 'Forest & Wildlife Resources', duration: '3.5 hours', progress: 45},
{title: 'Water Resources', duration: '3 hours', progress: 85},
{title: 'Agriculture', duration: '4 hours', progress: 25},
{title: 'Manufacturing Industries', duration: '4 hours', progress: 60},
]
};
const chapters = chapterData[subjectName] || [];
const modalContent = `
<div class="fixed inset-0 bg-black/50 flex items-center justify-center z-50" id="chapterModal">
<div class="bg-white rounded-lg w-full max-w-4xl mx-4 p-6 max-h-[90vh] overflow-y-auto">
<div class="flex justify-between items-center mb-6">
<h3 class="text-2xl font-bold text-gray-900">${subjectName} Chapters</h3>
<button class="w-10 h-10 flex items-center justify-center text-gray-500 hover:text-gray-700" onclick="closeChapterModal()">
<i class="ri-close-line ri-xl"></i>
</button>
</div>
<div class="space-y-4">
${chapters.map(chapter => `
<div class="bg-white border rounded-lg p-4 hover:shadow-lg transition-shadow">
<div class="flex items-center justify-between mb-2">
<h4 class="text-lg font-semibold text-gray-900">${chapter.title}</h4>
<span class="text-sm text-gray-500">${chapter.duration}</span>
</div>
<div class="relative pt-1">
<div class="flex mb-2 items-center justify-between">
<div>
<span class="text-xs font-semibold inline-block text-primary">
Progress: ${chapter.progress}%
</span>
</div>
</div>
<div class="overflow-hidden h-2 text-xs flex rounded bg-primary/10">
<div style="width:${chapter.progress}%" class="shadow-none flex flex-col text-center whitespace-nowrap text-white justify-center bg-primary transition-all duration-500"></div>
</div>
</div>
<div class="mt-4">
<div class="flex justify-between items-center mb-4">
<button class="px-4 py-2 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90 transition-colors ${chapter.progress === 100 ? 'opacity-50 cursor-not-allowed' : ''}" ${chapter.progress === 100 ? 'disabled' : ''}>
${chapter.progress === 0 ? 'Start Learning' : chapter.progress === 100 ? 'Completed' : 'Continue Learning'}
</button>
<div class="flex items-center gap-2">
<button class="w-8 h-8 flex items-center justify-center text-gray-500 hover:text-primary" onclick="showQuestionSuggestions('${subjectName}', '${chapter.title}')">
<i class="ri-question-line"></i>
</button>
<button class="w-8 h-8 flex items-center justify-center text-gray-500 hover:text-primary">
<i class="ri-download-line"></i>
</button>
<button class="w-8 h-8 flex items-center justify-center text-gray-500 hover:text-primary">
<i class="ri-bookmark-line"></i>
</button>
</div>
</div>
<div class="grid grid-cols-3 gap-4">
<div class="p-4 border rounded-lg hover:shadow-lg transition-all cursor-pointer">
<div class="flex items-center justify-between mb-2">
<h5 class="font-semibold text-gray-900">MCQ</h5>
</div>
<p class="text-sm text-gray-600">Multiple choice questions with detailed solutions</p>
</div>
<div class="p-4 border rounded-lg hover:shadow-lg transition-all cursor-pointer">
<div class="flex items-center justify-between mb-2">
<h5 class="font-semibold text-gray-900">SAQ</h5>
</div>
<p class="text-sm text-gray-600">Short answer questions with explanations</p>
</div>
<div class="p-4 border rounded-lg hover:shadow-lg transition-all cursor-pointer">
<div class="flex items-center justify-between mb-2">
<h5 class="font-semibold text-gray-900">Broad Questions</h5>
</div>
<p class="text-sm text-gray-600">Detailed questions with complete solutions</p>
</div>
</div>
</div>
</div>
`).join('')}
</div>
</div>
</div>
`;
document.body.insertAdjacentHTML('beforeend', modalContent);
document.body.style.overflow = 'hidden';
document.getElementById('chapterModal').addEventListener('click', (e) => {
if (e.target === document.getElementById('chapterModal')) {
closeChapterModal();
}
});
}
function closeChapterModal() {
const modal = document.getElementById('chapterModal');
if (modal) {
modal.remove();
document.body.style.overflow = 'auto';
}
}
function showQuestionSuggestions(subject, chapter) {
const questionData = {
'English': {
'First Flight (Prose)': [
{ type: 'MCQ', questions: [
{ question: 'What is the main theme of "A Letter to God"?', options: ['Faith', 'Greed', 'Love', 'War'], answer: 0, price: '₹10' },
{ question: 'Who is the protagonist in "Nelson Mandela: Long Walk to Freedom"?', options: ['Nelson Mandela', 'Gandhi', 'Martin Luther King', 'Malcolm X'], answer: 0, price: '₹10' }
]},
{ type: 'SAQ', questions: [
{ question: 'Explain the significance of the title "Fire and Ice"', answer: 'The poem explores two possible ways the world might end...', price: '₹20' },
{ question: 'Compare and contrast the two tigers in "Tiger in the Zoo"', answer: 'The poem presents two contrasting images...', price: '₹20' }
]},
{ type: 'Broad', questions: [
{ question: 'Critically analyze the themes of colonialism in "Nelson Mandela: Long Walk to Freedom"', answer: 'The text explores various aspects of colonialism...', price: '₹29' },
{ question: 'Discuss the symbolism used in "A Letter to God"', answer: 'The author uses various symbols throughout the story...', price: '₹29' }
]}
]
},
'Mathematics': {
'Real Numbers': [
{ question: 'Prove that √2 is irrational', difficulty: 'Hard' },
{ question: 'Find HCF of 336 and 54 using prime factorization', difficulty: 'Medium' },
{ question: 'Express 0.6666... as a rational number', difficulty: 'Medium' },
{ question: 'Find LCM of 12, 15 and 21', difficulty: 'Easy' },
{ question: 'Prove that 3 + 2√5 is irrational', difficulty: 'Hard' }
]
},
'Physics': {
'Mechanics': [
{ question: 'Derive the equation of motion v = u + at', difficulty: 'Hard' },
{ question: 'Calculate the force required to move a 10kg object with 2m/s² acceleration', difficulty: 'Medium' },
{ question: 'Explain Newton\'s First Law of Motion with examples', difficulty: 'Easy' },
{ question: 'Solve problems involving circular motion', difficulty: 'Hard' },
{ question: 'Define momentum and impulse', difficulty: 'Medium' }
]
}
};
const questions = questionData[subject]?.[chapter] || [];
if (questions.length === 0) return;
const modalContent = `
<div class="fixed inset-0 bg-black/50 flex items-center justify-center z-[60]" id="questionModal">
<div class="bg-white rounded-lg w-full max-w-4xl mx-4 p-6">
<div class="flex justify-between items-center mb-6">
<h3 class="text-2xl font-bold text-gray-900">Practice Questions - ${chapter}</h3>
<button class="w-10 h-10 flex items-center justify-center text-gray-500 hover:text-gray-700" onclick="closeQuestionModal()">
<i class="ri-close-line ri-xl"></i>
</button>
</div>
<div class="space-y-8">
${questions.map(section => `
<div class="bg-white border rounded-lg p-6">
<div class="flex items-center justify-between mb-4">
<h4 class="text-xl font-semibold text-gray-900">${section.type}</h4>
<span class="text-primary font-medium">${section.questions[0].price}</span>
</div>
<div class="space-y-6">
${section.questions.map(q => `
<div class="border-t pt-4">
<h5 class="text-lg text-gray-900 mb-4">${q.question}</h5>
${section.type === 'MCQ' ? `
<div class="space-y-2">
${q.options.map((option, idx) => `
<div class="flex items-center gap-3 p-3 border rounded-lg hover:bg-gray-50 cursor-pointer">
<input type="radio" name="q_${q.question}" id="opt_${idx}" class="w-4 h-4 text-primary">
<label for="opt_${idx}" class="text-gray-700 cursor-pointer">${option}</label>
</div>
`).join('')}
</div>
` : `
<div class="bg-gray-50 p-4 rounded-lg">
<p class="text-gray-600">${q.answer.substring(0, 100)}...</p>
<button class="mt-4 px-4 py-2 text-sm font-medium text-primary hover:text-primary/90">Read More</button>
</div>
`}
</div>
`).join('')}
</div>
${section.type === 'MCQ' ? `
<div class="mt-6 flex justify-end">
<button class="px-6 py-2 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90" onclick="showPaymentModal('${section.type}', '${section.questions[0].price}')">
Purchase Access (${section.questions[0].price})
</button>
</div>
` : ''}
</div>
`).join('')}
</div>
</div>
</div>
`;
document.body.insertAdjacentHTML('beforeend', modalContent);
}
function closeQuestionModal() {
const modal = document.getElementById('questionModal');
if (modal) {
modal.remove();
}
}
function showPaymentModal(type, price) {
// Remove payment modal functionality
}
function closePaymentModal() {
const modal = document.getElementById('paymentModal');
if (modal) {
modal.remove();
}
}
function handlePayment(method) {
  const paymentUrls = {
    phonepe: 'phonepe://',
    googlepay: 'tez://',
    paytm: 'paytmmp://',
    paypal: 'https://www.paypal.com/signin'
  };

  const paymentDetailsModal = `
    <div class="fixed inset-0 bg-black/50 flex items-center justify-center z-[80]" id="paymentDetailsModal">
      <div class="bg-white rounded-lg w-full max-w-md mx-4 p-6">
        <div class="flex justify-between items-center mb-6">
          <h3 class="text-2xl font-bold text-gray-900">Payment Details</h3>
          <button class="w-10 h-10 flex items-center justify-center text-gray-500 hover:text-gray-700" onclick="closePaymentDetailsModal()">
            <i class="ri-close-line ri-xl"></i>
          </button>
        </div>
        <form onsubmit="processPayment(event)" class="space-y-4">
          <div class="space-y-2">
            <label class="block text-sm font-medium text-gray-700">Transaction ID</label>
            <input type="text" id="transactionId" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-primary/20 focus:border-primary outline-none" required>
          </div>
          <button type="submit" class="w-full px-6 py-3 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90">
            Verify Payment
          </button>
        </form>
        <div class="mt-6 text-center">
          <p class="text-sm text-gray-500">Please complete the payment in your ${method} app and enter the transaction ID here.</p>
          <a href="${paymentUrls[method]}" target="_blank" class="mt-2 inline-block text-primary hover:text-primary/90">
            Open ${method.charAt(0).toUpperCase() + method.slice(1)}
          </a>
        </div>
      </div>
    </div>
  `;
  
  closePaymentModal();
  document.body.insertAdjacentHTML('beforeend', paymentDetailsModal);
}
function closePaymentDetailsModal() {
const modal = document.getElementById('paymentDetailsModal');
if (modal) {
modal.remove();
}
}
function processPayment(event) {
  event.preventDefault();
  const transactionId = document.getElementById('transactionId').value;
  
  // Here you would typically verify the transaction with your backend
  // For demo purposes, we'll simulate a successful payment
  verifyPayment(transactionId);
}

function verifyPayment(transactionId) {
  // Simulate payment verification
  const successModal = `
    <div class="fixed inset-0 bg-black/50 flex items-center justify-center z-[90]" id="successModal">
      <div class="bg-white rounded-lg w-full max-w-md mx-4 p-6 text-center">
        <div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center bg-green-100 rounded-full">
          <i class="ri-check-line ri-2x text-green-500"></i>
        </div>
        <h3 class="text-2xl font-bold text-gray-900 mb-2">Payment Successful!</h3>
        <p class="text-gray-600 mb-6">Your payment has been verified. You can now access the content.</p>
        <div class="space-y-4">
          <button onclick="downloadPDF()" class="w-full px-6 py-3 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90">
            Download PDF
          </button>
          <button onclick="closeAllModals()" class="w-full px-6 py-3 border text-gray-700 font-semibold !rounded-button hover:bg-gray-50">
            Close
          </button>
        </div>
      </div>
    </div>
  `;
  
  closePaymentDetailsModal();
  document.body.insertAdjacentHTML('beforeend', successModal);
}

function downloadPDF() {
  // Here you would implement the actual PDF download logic
  // For now, we'll show a message
  const notification = document.createElement('div');
  notification.className = 'fixed bottom-4 right-4 bg-green-500 text-white px-6 py-3 rounded-lg shadow-lg';
  notification.textContent = 'PDF download started...';
  document.body.appendChild(notification);
  
  setTimeout(() => {
    notification.remove();
  }, 3000);
}
function verifyPayment() {
// Remove payment verification functionality
}
function showAuthModal(type) {
const modalContent = `
<div class="fixed inset-0 bg-black/50 flex items-center justify-center z-[100]" id="authModal">
<div class="bg-white rounded-lg w-full max-w-md mx-4 p-6">
<div class="flex justify-between items-center mb-6">
<h3 class="text-2xl font-bold text-gray-900">${type === 'signin' ? 'Sign In' : 'Create Account'}</h3>
<button class="w-10 h-10 flex items-center justify-center text-gray-500 hover:text-gray-700" onclick="closeAuthModal()">
<i class="ri-close-line ri-xl"></i>
</button>
</div>
<form class="space-y-4" onsubmit="handleAuth(event, '${type}')">
${type === 'signup' ? `
<div class="space-y-2">
<label class="block text-sm font-medium text-gray-700">Full Name</label>
<input type="text" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-primary/20 focus:border-primary outline-none" placeholder="Enter your full name" required>
</div>
` : ''}
<div class="space-y-2">
<label class="block text-sm font-medium text-gray-700">Email</label>
<input type="email" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-primary/20 focus:border-primary outline-none" placeholder="Enter your email" required>
</div>
<div class="space-y-2">
<label class="block text-sm font-medium text-gray-700">Password</label>
<input type="password" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-primary/20 focus:border-primary outline-none" placeholder="Enter your password" required>
</div>
${type === 'signup' ? `
<div class="space-y-2">
<label class="block text-sm font-medium text-gray-700">Confirm Password</label>
<input type="password" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-primary/20 focus:border-primary outline-none" placeholder="Confirm your password" required>
</div>
` : ''}
<button type="submit" class="w-full px-6 py-3 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90">
${type === 'signin' ? 'Sign In' : 'Create Account'}
</button>
</form>
<div class="mt-6">
<div class="relative">
<div class="absolute inset-0 flex items-center">
<div class="w-full border-t border-gray-300"></div>
</div>
<div class="relative flex justify-center text-sm">
<span class="px-2 bg-white text-gray-500">Or continue with</span>
</div>
</div>
<div class="mt-6 grid grid-cols-3 gap-3">
<button class="w-full flex items-center justify-center px-4 py-2 border rounded-lg hover:bg-gray-50">
<i class="ri-google-fill ri-xl text-[#4285F4]"></i>
</button>
<button class="w-full flex items-center justify-center px-4 py-2 border rounded-lg hover:bg-gray-50">
<i class="ri-facebook-fill ri-xl text-[#1877F2]"></i>
</button>
<button class="w-full flex items-center justify-center px-4 py-2 border rounded-lg hover:bg-gray-50">
<i class="ri-apple-fill ri-xl"></i>
</button>
</div>
</div>
<p class="mt-6 text-center text-sm text-gray-500">
${type === 'signin' ? "Don't have an account?" : 'Already have an account?'}
<button onclick="switchAuthMode('${type === 'signin' ? 'signup' : 'signin'}')" class="font-medium text-primary hover:text-primary/90">
${type === 'signin' ? 'Sign up' : 'Sign in'}
</button>
</p>
</div>
</div>
`;
document.body.insertAdjacentHTML('beforeend', modalContent);
}
function closeAuthModal() {
const modal = document.getElementById('authModal');
if (modal) {
modal.remove();
}
}
function switchAuthMode(type) {
closeAuthModal();
showAuthModal(type);
}
function handleAuth(event, type) {
event.preventDefault();
const successModal = `
<div class="fixed inset-0 bg-black/50 flex items-center justify-center z-[110]" id="authSuccessModal">
<div class="bg-white rounded-lg w-full max-w-md mx-4 p-6 text-center">
<div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center bg-green-100 rounded-full">
<i class="ri-check-line ri-2x text-green-500"></i>
</div>
<h3 class="text-2xl font-bold text-gray-900 mb-2">${type === 'signin' ? 'Welcome Back!' : 'Account Created!'}</h3>
<p class="text-gray-600 mb-6">${type === 'signin' ? 'You have successfully signed in.' : 'Your account has been created successfully.'}</p>
<button onclick="closeAllModals()" class="px-6 py-3 bg-primary text-white font-semibold !rounded-button hover:bg-primary/90">
Continue
</button>
</div>
</div>
`;
document.body.insertAdjacentHTML('beforeend', successModal);
closeAuthModal();
}
function closeAllModals() {
const modals = ['successModal', 'paymentDetailsModal', 'paymentModal', 'questionModal', 'authModal', 'authSuccessModal'];
modals.forEach(modalId => {
const modal = document.getElementById(modalId);
if (modal) {
modal.remove();
}
});
}
document.getElementById('subjectModal').addEventListener('click', (e) => {
if (e.target === document.getElementById('subjectModal')) {
closeSubjectModal();
}
});
</script>
</body>
</html>
