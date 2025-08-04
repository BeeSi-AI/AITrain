<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Train | Beginner Courses in Artificial Intelligence</title>
    <style>
        /* CSS Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(135deg, #6e8efb, #a777e3);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 1rem;
        }
        
        .logo-area {
            width: 150px;
            height: 150px;
            background-color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            margin-bottom: 1rem;
            border: 3px solid white;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        .logo-area img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .logo-upload {
            display: none;
            margin-top: 0.5rem;
        }
        
        .logo-upload input {
            display: none;
        }
        
        .upload-btn {
            background-color: rgba(255, 255, 255, 0.2);
            color: white;
            border: none;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        .upload-btn:hover {
            background-color: rgba(255, 255, 255, 0.3);
        }
        
        .container {
            width: 85%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 0;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        h2 {
            font-size: 2rem;
            margin: 2rem 0 1.5rem;
            color: #444;
        }
        
        h3 {
            font-size: 1.5rem;
            margin: 1.5rem 0 1rem;
            color: #555;
        }
        
        p {
            margin-bottom: 1rem;
        }
        
        .hero {
            text-align: center;
            padding: 3rem 0;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: #6e8efb;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            margin: 0.5rem;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: #5a7df7;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(110, 142, 251, 0.3);
        }
        
        .btn-secondary {
            background-color: #e0e0e0;
            color: #333;
        }
        
        .btn-secondary:hover {
            background-color: #d0d0d0;
        }
        
        .courses {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }
        
        .course-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
            position: relative;
        }
        
        .course-card:hover {
            transform: translateY(-10px);
        }
        
        .course-img {
            height: 180px;
            background-color: #e0e0e0;
            background-size: cover;
            background-position: center;
        }
        
        .course-content {
            padding: 1.5rem;
        }
        
        .course-price {
            font-weight: bold;
            color: #6e8efb;
            font-size: 1.2rem;
            margin: 0.5rem 0;
        }
        
        .features {
            background-color: #f1f5f9;
            padding: 3rem 0;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .feature {
            text-align: center;
            padding: 1.5rem;
        }
        
        .feature i {
            font-size: 3rem;
            color: #6e8efb;
            margin-bottom: 1rem;
        }
        
        .testimonials {
            padding: 3rem 0;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .testimonial {
            background: white;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .testimonial-author {
            font-weight: bold;
            margin-top: 1rem;
            color: #6e8efb;
        }
        
        footer {
            background-color: #333;
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .cta {
            background: linear-gradient(135deg, #a777e3, #6e8efb);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }
        
        /* Admin Panel Styles */
        .admin-panel {
            background-color: white;
            border-radius: 10px;
            padding: 1.5rem;
            margin-top: 1.5rem;
            display: none;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .form-group {
            margin-bottom: 1rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }
        
        .form-group input, 
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        
        .materials-list {
            margin-top: 1rem;
        }
        
        .material-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.5rem;
            background-color: #f8f9fa;
            border-radius: 5px;
            margin-bottom: 0.5rem;
        }
        
        .video-container {
            margin-top: 1rem;
        }
        
        .video-item {
            margin-bottom: 1rem;
        }
        
        .certificate-container {
            background: white;
            border-radius: 10px;
            padding: 2rem;
            max-width: 800px;
            margin: 2rem auto;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            display: none;
        }
        
        .certificate-header {
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .certificate-title {
            font-size: 2.5rem;
            color: #6e8efb;
            margin: 0.5rem 0;
        }
        
        .certificate-body {
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .student-name {
            font-size: 1.8rem;
            font-weight: bold;
            margin: 1rem 0;
            color: #333;
        }
        
        .course-name {
            font-size: 1.4rem;
            margin: 1rem 0;
            color: #6e8efb;
        }
        
        .certificate-footer {
            display: flex;
            justify-content: space-between;
            margin-top: 2rem;
        }
        
        .signature {
            text-align: center;
        }
        
        .date {
            text-align: center;
            font-style: italic;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            h2 {
                font-size: 1.7rem;
            }
            .container {
                width: 95%;
            }
        }
    </style>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="logo-container">
                <div class="logo-area" id="logoDisplay">
                    <!-- Logo will be displayed here -->
                    <img src="" alt="AI Train Logo" style="display: none;">
                </div>
                <div class="logo-upload">
                    <input type="file" id="logoUpload" accept="image/jpeg, image/png, image/jpg">
                    <button class="upload-btn" id="uploadLogoBtn">Change Logo</button>
                </div>
                <h1>AI Train</h1>
                <p>Begin your journey into Artificial Intelligence with our beginner-friendly courses</p>
            </div>
        </div>
    </header>
    
    <section class="hero">
        <div class="container">
            <h2>Start Your AI Journey Today</h2>
            <p>Our carefully designed courses make learning Artificial Intelligence accessible to everyone, regardless of your background. No prior experience required!</p>
            <a href="#courses" class="btn">Explore Courses</a>
            <a href="#signup" class="btn">Get Started</a>
            <button class="btn btn-secondary" id="adminModeBtn">Admin Mode</button>
        </div>
    </section>
    
    <section id="courses" class="container">
        <h2>Our Beginner Courses</h2>
        <p>Start with the fundamentals and build a strong foundation in AI concepts and applications.</p>
        
        <div class="courses">
            <!-- Course 1 -->
            <div class="course-card" data-course-id="1">
                <div class="course-img" style="background-image: url('https://source.unsplash.com/random/300x180/?ai,artificial-intelligence');"></div>
                <div class="course-content">
                    <h3>Introduction to AI & Machine Learning</h3>
                    <p class="course-description">Learn the fundamental concepts of artificial intelligence and machine learning, including how AI systems work and their real-world applications.</p>
                    <p><strong>Duration:</strong> 6 weeks</p>
                    <p><strong>Format:</strong> Online, self-paced</p>
                    <p class="course-price">Free</p>
                    
                    <!-- Admin Controls -->
                    <div class="admin-controls" style="display: none;">
                        <button class="btn btn-secondary edit-course-btn">Edit Description</button>
                    </div>
                    
                    <!-- Admin Panel for Editing -->
                    <div class="admin-panel">
                        <h3>Edit Course Description</h3>
                        <div class="form-group">
                            <label for="course-description-1">Description</label>
                            <textarea id="course-description-1" rows="4" class="course-description-input">Learn the fundamental concepts of artificial intelligence and machine learning, including how AI systems work and their real-world applications.</textarea>
                        </div>
                        <button class="btn save-description-btn" data-course-id="1">Save Description</button>
                        
                        <!-- Add Materials -->
                        <h3 style="margin-top: 1.5rem;">Add Course Material</h3>
                        <div class="form-group">
                            <label for="material-title-1">Material Title</label>
                            <input type="text" id="material-title-1" placeholder="Enter material title">
                        </div>
                        <div class="form-group">
                            <label for="material-file-1">Upload File</label>
                            <input type="file" id="material-file-1">
                        </div>
                        <button class="btn add-material-btn" data-course-id="1">Add Material</button>
                        
                        <!-- Materials List -->
                        <div class="materials-list" id="materials-list-1">
                            <!-- Materials will be added here -->
                        </div>
                        
                        <!-- Add Videos -->
                        <h3 style="margin-top: 1.5rem;">Add Video</h3>
                        <div class="form-group">
                            <label for="video-title-1">Video Title</label>
                            <input type="text" id="video-title-1" placeholder="Enter video title">
                        </div>
                        <div class="form-group">
                            <label for="video-url-1">YouTube/Vimeo URL</label>
                            <input type="url" id="video-url-1" placeholder="https://www.youtube.com/watch?v=...">
                        </div>
                        <button class="btn add-video-btn" data-course-id="1">Add Video</button>
                        
                        <!-- Videos List -->
                        <div class="video-container" id="videos-container-1">
                            <!-- Videos will be added here -->
                        </div>
                    </div>
                    
                    <a href="#" class="btn enroll-btn">Enroll Now</a>
                    <button class="btn complete-course-btn" style="display: none;">Complete Course</button>
                </div>
            </div>
            
            <!-- Course 2 -->
            <div class="course-card" data-course-id="2">
                <div class="course-img" style="background-image: url('https://source.unsplash.com/random/300x180/?python,code');"></div>
                <div class="course-content">
                    <h3>Python for AI Beginners</h3>
                    <p class="course-description">Master the Python programming skills needed for AI development, with a focus on libraries like NumPy, Pandas, and basic data manipulation.</p>
                    <p><strong>Duration:</strong> 8 weeks</p>
                    <p><strong>Format:</strong> Online with live sessions</p>
                    <p class="course-price">$99</p>
                    
                    <!-- Admin Controls -->
                    <div class="admin-controls" style="display: none;">
                        <button class="btn btn-secondary edit-course-btn">Edit Description</button>
                    </div>
                    
                    <!-- Admin Panel for Editing -->
                    <div class="admin-panel">
                        <h3>Edit Course Description</h3>
                        <div class="form-group">
                            <label for="course-description-2">Description</label>
                            <textarea id="course-description-2" rows="4" class="course-description-input">Master the Python programming skills needed for AI development, with a focus on libraries like NumPy, Pandas, and basic data manipulation.</textarea>
                        </div>
                        <button class="btn save-description-btn" data-course-id="2">Save Description</button>
                        
                        <!-- Add Materials -->
                        <h3 style="margin-top: 1.5rem;">Add Course Material</h3>
                        <div class="form-group">
                            <label for="material-title-2">Material Title</label>
                            <input type="text" id="material-title-2" placeholder="Enter material title">
                        </div>
                        <div class="form-group">
                            <label for="material-file-2">Upload File</label>
                            <input type="file" id="material-file-2">
                        </div>
                        <button class="btn add-material-btn" data-course-id="2">Add Material</button>
                        
                        <!-- Materials List -->
                        <div class="materials-list" id="materials-list-2">
                            <!-- Materials will be added here -->
                        </div>
                        
                        <!-- Add Videos -->
                        <h3 style="margin-top: 1.5rem;">Add Video</h3>
                        <div class="form-group">
                            <label for="video-title-2">Video Title</label>
                            <input type="text" id="video-title-2" placeholder="Enter video title">
                        </div>
                        <div class="form-group">
                            <label for="video-url-2">YouTube/Vimeo URL</label>
                            <input type="url" id="video-url-2" placeholder="https://www.youtube.com/watch?v=...">
                        </div>
                        <button class="btn add-video-btn" data-course-id="2">Add Video</button>
                        
                        <!-- Videos List -->
                        <div class="video-container" id="videos-container-2">
                            <!-- Videos will be added here -->
                        </div>
                    </div>
                    
                    <a href="#" class="btn enroll-btn">Enroll Now</a>
                    <button class="btn complete-course-btn" style="display: none;">Complete Course</button>
                </div>
            </div>
            
            <!-- Course 3 -->
            <div class="course-card" data-course-id="3">
                <div class="course-img" style="background-image: url('https://source.unsplash.com/random/300x180/?data,science');"></div>
                <div class="course-content">
                    <h3>Data Science Fundamentals</h3>
                    <p class="course-description">Understand how data drives AI systems. Learn data collection, cleaning, visualization, and basic statistical analysis for AI applications.</p>
                    <p><strong>Duration:</strong> 10 weeks</p>
                    <p><strong>Format:</strong> Online, self-paced</p>
                    <p class="course-price">$149</p>
                    
                    <!-- Admin Controls -->
                    <div class="admin-controls" style="display: none;">
                        <button class="btn btn-secondary edit-course-btn">Edit Description</button>
                    </div>
                    
                    <!-- Admin Panel for Editing -->
                    <div class="admin-panel">
                        <h3>Edit Course Description</h3>
                        <div class="form-group">
                            <label for="course-description-3">Description</label>
                            <textarea id="course-description-3" rows="4" class="course-description-input">Understand how data drives AI systems. Learn data collection, cleaning, visualization, and basic statistical analysis for AI applications.</textarea>
                        </div>
                        <button class="btn save-description-btn" data-course-id="3">Save Description</button>
                        
                        <!-- Add Materials -->
                        <h3 style="margin-top: 1.5rem;">Add Course Material</h3>
                        <div class="form-group">
                            <label for="material-title-3">Material Title</label>
                            <input type="text" id="material-title-3" placeholder="Enter material title">
                        </div>
                        <div class="form-group">
                            <label for="material-file-3">Upload File</label>
                            <input type="file" id="material-file-3">
                        </div>
                        <button class="btn add-material-btn" data-course-id="3">Add Material</button>
                        
                        <!-- Materials List -->
                        <div class="materials-list" id="materials-list-3">
                            <!-- Materials will be added here -->
                        </div>
                        
                        <!-- Add Videos -->
                        <h3 style="margin-top: 1.5rem;">Add Video</h3>
                        <div class="form-group">
                            <label for="video-title-3">Video Title</label>
                            <input type="text" id="video-title-3" placeholder="Enter video title">
                        </div>
                        <div class="form-group">
                            <label for="video-url-3">YouTube/Vimeo URL</label>
                            <input type="url" id="video-url-3" placeholder="https://www.youtube.com/watch?v=...">
                        </div>
                        <button class="btn add-video-btn" data-course-id="3">Add Video</button>
                        
                        <!-- Videos List -->
                        <div class="video-container" id="videos-container-3">
                            <!-- Videos will be added here -->
                        </div>
                    </div>
                    
                    <a href="#" class="btn enroll-btn">Enroll Now</a>
                    <button class="btn complete-course-btn" style="display: none;">Complete Course</button>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Certificate Template -->
    <div class="certificate-container" id="certificate-template">
        <div class="certificate-header">
            <h2>AI Train</h2>
            <div class="certificate-title">Certificate of Completion</div>
        </div>
        
        <div class="certificate-body">
            <p>This is to certify that</p>
            <div class="student-name" id="certificate-student-name">John Doe</div>
            <p>has successfully completed the course</p>
            <div class="course-name" id="certificate-course-name">Introduction to AI & Machine Learning</div>
            <p>with dedication and excellence</p>
        </div>
        
        <div class="certificate-footer">
            <div class="signature">
                <p>Signature</p>
                <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDAiIGhlaWdodD0iNTAiIHZpZXdCb3g9IjAgMCAxMDAgNTAiPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9IiNmZmYiLz48cGF0aCBkPSJNNSwzMCBDMTAsMTAgMjAsMTAgMzAsMjAgQzQwLDMwIDUwLDEwIDYwLDIwIEM3MCwzMCA4MCwxMCA5MCwzMCIgc3Ryb2tlPSIjMDAwIiBzdHJva2Utd2lkdGg9IjIiIGZpbGw9Im5vbmUiLz48L3N2Zz4=" alt="Digital Signature" style="height: 50px;">
                <p>AI Train Director</p>
            </div>
            <div class="date">
                <p>Date: <span id="certificate-date">June 15, 2023</span></p>
            </div>
        </div>
    </div>
    
    <section class="features">
        <div class="container">
            <h2>Why Learn With Us?</h2>
            <div class="features-grid">
                <div class="feature">
                    <i class="fas fa-graduation-cap"></i>
                    <h3>Expert Instructors</h3>
                    <p>Learn from industry professionals and academic experts with real-world AI experience.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-laptop-code"></i>
                    <h3>Hands-On Projects</h3>
                    <p>Apply your knowledge through practical exercises and real-world projects.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-users"></i>
                    <h3>Supportive Community</h3>
                    <p>Join a network of learners and participate in discussion forums and study groups.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-certificate"></i>
                    <h3>Certificate of Completion</h3>
                    <p>Receive a shareable certificate to showcase your new skills to employers.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section class="testimonials">
        <div class="container">
            <h2>What Our Students Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial">
                    <p>"I had no background in programming, but the Introduction to AI course was perfectly paced and incredibly informative. I now feel confident to explore more advanced topics!"</p>
                    <p class="testimonial-author">- Sarah Johnson, Course Graduate</p>
                </div>
                <div class="testimonial">
                    <p>"The Python for AI course transformed my understanding of programming. The hands-on exercises made complex concepts easy to grasp. Highly recommend for absolute beginners!"</p>
                    <p class="testimonial-author">- Michael Chen, Data Analyst</p>
                </div>
                <div class="testimonial">
                    <p>"As a career changer, I needed a structured way to learn AI fundamentals. These courses provided exactly what I needed to start my new journey in tech."</p>
                    <p class="testimonial-author">- Emma Rodriguez, Career Changer</p>
                </div>
            </div>
        </div>
    </section>
    
    <section class="cta" id="signup">
        <div class="container">
            <h2>Ready to Begin Your AI Journey?</h2>
            <p>Join thousands of students who have started their AI education with our beginner courses.</p>
            <a href="#" class="btn">Sign Up Now</a>
            <p style="margin-top: 1rem; font-size: 0.9rem;">30-day money-back guarantee • Flexible learning schedule • Lifetime access to course materials</p>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <p>&copy; 2023 AI Train. All rights reserved.</p>
            <p>Contact us: info@aitrain.com | (555) 123-4567</p>
        </div>
    </footer>

    <script>
        // Logo upload functionality
        document.addEventListener('DOMContentLoaded', function() {
            const logoUpload = document.getElementById('logoUpload');
            const uploadLogoBtn = document.getElementById('uploadLogoBtn');
            const logoDisplay = document.getElementById('logoDisplay');
            const logoImg = logoDisplay.querySelector('img');
            
            // Admin mode toggle
            const adminModeBtn = document.getElementById('adminModeBtn');
            let adminMode = false;
            
            adminModeBtn.addEventListener('click', function() {
                adminMode = !adminMode;
                adminModeBtn.textContent = adminMode ? 'User Mode' : 'Admin Mode';
                adminModeBtn.style.background = adminMode ? '#e0e0e0' : '#6e8efb';
                
                // Show/hide admin controls for all courses
                document.querySelectorAll('.admin-controls').forEach(el => {
                    el.style.display = adminMode ? 'block' : 'none';
                });
                
                // Show/hide complete course buttons
                document.querySelectorAll('.complete-course-btn').forEach(el => {
                    el.style.display = adminMode ? 'inline-block' : 'none';
                });
            });
            
            // Show logo upload controls on hover
            logoDisplay.addEventListener('mouseenter', function() {
                if (adminMode) {
                    document.querySelector('.logo-upload').style.display = 'block';
                }
            });
            
            logoDisplay.addEventListener('mouseleave', function() {
                // Keep visible if hovering over the upload button
                setTimeout(() => {
                    if (!document.querySelector('.logo-upload:hover')) {
                        document.querySelector('.logo-upload').style.display = 'none';
                    }
                }, 200);
            });
            
            // Handle logo upload
            uploadLogoBtn.addEventListener('click', function() {
                if (adminMode) {
                    logoUpload.click();
                }
            });
            
            logoUpload.addEventListener('change', function(e) {
                if (adminMode && e.target.files && e.target.files[0]) {
                    const reader = new FileReader();
                    
                    reader.onload = function(event) {
                        // Display the image
                        logoImg.src = event.target.result;
                        logoImg.style.display = 'block';
                        
                        // Save to localStorage
                        localStorage.setItem('aiTrainLogo', event.target.result);
                    }
                    
                    reader.readAsDataURL(e.target.files[0]);
                }
            });
            
            // Load logo from localStorage if exists
            const savedLogo = localStorage.getItem('aiTrainLogo');
            if (savedLogo) {
                logoImg.src = savedLogo;
                logoImg.style.display = 'block';
            }
            
            // Course description editing functionality
            document.querySelectorAll('.edit-course-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const courseCard = this.closest('.course-card');
                    const adminPanel = courseCard.querySelector('.admin-panel');
                    adminPanel.style.display = adminPanel.style.display === 'block' ? 'none' : 'block';
                });
            });
            
            // Save course description
            document.querySelectorAll('.save-description-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const courseId = this.getAttribute('data-course-id');
                    const textarea = document.getElementById(`course-description-${courseId}`);
                    const courseDescription = document.querySelector(`.course-card[data-course-id="${courseId}"] .course-description`);
                    
                    if (courseDescription && textarea) {
                        courseDescription.textContent = textarea.value;
                        alert('Course description updated successfully!');
                    }
                });
            });
            
            // Add course material
            document.querySelectorAll('.add-material-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const courseId = this.getAttribute('data-course-id');
                    const titleInput = document.getElementById(`material-title-${courseId}`);
                    const fileInput = document.getElementById(`material-file-${courseId}`);
                    const materialsList = document.getElementById(`materials-list-${courseId}`);
                    
                    if (titleInput && titleInput.value.trim() !== '') {
                        const materialItem = document.createElement('div');
                        materialItem.className = 'material-item';
                        
                        const titleSpan = document.createElement('span');
                        titleSpan.textContent = titleInput.value;
                        
                        const downloadBtn = document.createElement('a');
                        downloadBtn.href = '#';
                        downloadBtn.className = 'btn btn-secondary';
                        downloadBtn.style.fontSize = '0.8rem';
                        downloadBtn.textContent = 'Download';
                        
                        materialItem.appendChild(titleSpan);
                        materialItem.appendChild(downloadBtn);
                        materialsList.appendChild(materialItem);
                        
                        // Reset inputs
                        titleInput.value = '';
                        
                        alert('Material added successfully!');
                    }
                });
            });
            
            // Add video
            document.querySelectorAll('.add-video-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const courseId = this.getAttribute('data-course-id');
                    const titleInput = document.getElementById(`video-title-${courseId}`);
                    const urlInput = document.getElementById(`video-url-${courseId}`);
                    const videosContainer = document.getElementById(`videos-container-${courseId}`);
                    
                    if (titleInput && titleInput.value.trim() !== '' && urlInput && urlInput.value.trim() !== '') {
                        const videoItem = document.createElement('div');
                        videoItem.className = 'video-item';
                        
                        const videoTitle = document.createElement('h4');
                        videoTitle.textContent = titleInput.value;
                        
                        // Extract video ID from URL (works for YouTube)
                        let videoId = '';
                        const youtubeMatch = urlInput.value.match(/(?:youtube\.com\/watch\?v=|youtu\.be\/|youtube\.com\/embed\/)([^&\n?#]+)/);
                        if (youtubeMatch && youtubeMatch[1]) {
                            videoId = youtubeMatch[1];
                        }
                        
                        let videoElement;
                        if (videoId) {
                            // Use YouTube embed
                            videoElement = document.createElement('iframe');
                            videoElement.width = '100%';
                            videoElement.height = '200';
                            videoElement.src = `https://www.youtube.com/embed/${videoId}`;
                            videoElement.frameBorder = '0';
                            videoElement.allowFullscreen = true;
                        } else {
                            // For other video platforms
                            videoElement = document.createElement('div');
                            videoElement.innerHTML = `<a href="${urlInput.value}" target="_blank">Watch Video</a>`;
                        }
                        
                        const removeBtn = document.createElement('button');
                        removeBtn.className = 'btn btn-secondary';
                        removeBtn.style.fontSize = '0.8rem';
                        removeBtn.textContent = 'Remove';
                        removeBtn.addEventListener('click', function() {
                            videosContainer.removeChild(videoItem);
                        });
                        
                        videoItem.appendChild(videoTitle);
                        videoItem.appendChild(videoElement);
                        videoItem.appendChild(removeBtn);
                        videosContainer.appendChild(videoItem);
                        
                        // Reset inputs
                        titleInput.value = '';
                        urlInput.value = '';
                        
                        alert('Video added successfully!');
                    }
                });
            });
            
            // Complete course and generate certificate
            document.querySelectorAll('.complete-course-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const courseCard = this.closest('.course-card');
                    const courseTitle = courseCard.querySelector('h3').textContent;
                    
                    // Show certificate
                    const certificate = document.getElementById('certificate-template');
                    document.getElementById('certificate-course-name').textContent = courseTitle;
                    document.getElementById('certificate-student-name').textContent = 'John Doe'; // In a real app, this would be the logged-in user's name
                    
                    // Set current date
                    const now = new Date();
                    const options = { year: 'numeric', month: 'long', day: 'numeric' };
                    document.getElementById('certificate-date').textContent = now.toLocaleDateString(undefined, options);
                    
                    certificate.style.display = 'block';
                    
                    // Scroll to certificate
                    certificate.scrollIntoView({ behavior: 'smooth' });
                });
            });
        });
    </script>
</body>
</html>
