# kreeshna3310.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bharatbinary - Custom Software Solutions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        .page-section {
            display: none;
            animation: fadeIn 0.5s ease-in;
        }
        
        .page-section.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .nav-active {
            color: #2563eb;
            font-weight: 600;
            border-bottom: 2px solid #2563eb;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .service-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .form-input:focus {
            outline: none;
            border-color: #2563eb;
            box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <span class="text-2xl font-bold text-blue-600">Sudhesh Bavade Enterprize</span>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <button onclick="showPage('home')" class="text-gray-700 hover:text-blue-600 px-3 py-2 nav-active">Home</button>
                    <button onclick="showPage('services')" class="text-gray-700 hover:text-blue-600 px-3 py-2">Services</button>
                    <button onclick="showPage('about')" class="text-gray-700 hover:text-blue-600 px-3 py-2">About</button>
                    <button onclick="showPage('contact')" class="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition-colors">Get Quote</button>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-button" class="text-gray-700">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white shadow-lg">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <button onclick="showPage('home')" class="block w-full text-left px-3 py-2 text-gray-700 hover:bg-blue-50 hover:text-blue-600 rounded nav-active">Home</button>
                <button onclick="showPage('services')" class="block w-full text-left px-3 py-2 text-gray-700 hover:bg-blue-50 hover:text-blue-600 rounded">Services</button>
                <button onclick="showPage('about')" class="block w-full text-left px-3 py-2 text-gray-700 hover:bg-blue-50 hover:text-blue-600 rounded">About</button>
                <button onclick="showPage('contact')" class="block w-full text-left px-3 py-2 bg-blue-600 text-white rounded hover:bg-blue-700">Get Quote</button>
            </div>
        </div>
    </nav>

    <!-- Home Page -->
    <section id="home" class="page-section active pt-16">
        <!-- Hero Section -->
        <div class="gradient-bg text-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div>
                        <h1 class="text-4xl md:text-5xl font-bold mb-6">Transform Your Vision Into Digital Reality</h1>
                        <p class="text-xl mb-8 opacity-90">Custom software solutions tailored to your unique business needs. From concept to deployment, we build with precision.</p>
                        <div class="flex flex-wrap gap-4">
                            <button onclick="showPage('contact')" class="bg-white text-blue-600 px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition-colors">
                                Start Your Project
                            </button>
                            <button onclick="showPage('services')" class="border-2 border-white text-white px-8 py-3 rounded-lg font-semibold hover:bg-white hover:text-blue-600 transition-colors">
                                Explore Services
                            </button>
                        </div>
                    </div>
                    <div class="flex justify-center">
                        <img src="https://placehold.co/600x400" alt="Modern software development workspace showing multiple screens with code and design interfaces, collaborative team environment" class="rounded-lg shadow-2xl" />
                    </div>
                </div>
            </div>
        </div>

        <!-- Stats Section -->
        <div class="bg-white py-16">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
                    <div>
                        <div class="text-3xl md:text-4xl font-bold text-blue-600 mb-2">50+</div>
                        <div class="text-gray-600">Projects Completed</div>
                    </div>
                    <div>
                        <div class="text-3xl md:text-4xl font-bold text-blue-600 mb-2">15+</div>
                        <div class="text-gray-600">Happy Clients</div>
                    </div>
                    <div>
                        <div class="text-3xl md:text-4xl font-bold text-blue-600 mb-2">3+</div>
                        <div class="text-gray-600">Years Experience</div>
                    </div>
                    <div>
                        <div class="text-3xl md:text-4xl font-bold text-blue-600 mb-2">24/7</div>
                        <div class="text-gray-600">Support</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Featured Services Preview -->
        <div class="bg-gray-50 py-16">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold text-gray-800 mb-4">Our Core Services</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">We offer comprehensive software development services to bring your ideas to life</p>
                </div>
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="service-card bg-white p-6 rounded-lg shadow-md">
                        <div class="text-blue-600 text-3xl mb-4">
                            <i class="fas fa-globe"></i>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Web Development</h3>
                        <p class="text-gray-600 mb-4">Custom websites and web applications built with modern technologies and responsive design.</p>
                        <button onclick="showPage('services')" class="text-blue-600 font-semibold hover:text-blue-700">
                            Learn More →
                        </button>
                    </div>
                    <div class="service-card bg-white p-6 rounded-lg shadow-md">
                        <div class="text-blue-600 text-3xl mb-4">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Mobile Apps</h3>
                        <p class="text-gray-600 mb-4">Native and cross-platform mobile applications for iOS and Android with seamless user experience.</p>
                        <button onclick="showPage('services')" class="text-blue-600 font-semibold hover:text-blue-700">
                            Learn More →
                        </button>
                    </div>
                    <div class="service-card bg-white p-6 rounded-lg shadow-md">
                        <div class="text-blue-600 text-3xl mb-4">
                            <i class="fas fa-cogs"></i>
                        </div>
                        <h3 class="text-xl font-semibold mb-3">Custom Software</h3>
                        <p class="text-gray-600 mb-4">Tailored software solutions designed specifically for your business processes and requirements.</p>
                        <button onclick="showPage('services')" class="text-blue-600 font-semibold hover:text-blue-700">
                            Learn More →
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Page -->
    <section id="services" class="page-section pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="text-center mb-16">
                <h1 class="text-4xl font-bold text-gray-800 mb-4">Our Services</h1>
                <p class="text-gray-600 max-w-2xl mx-auto">Comprehensive software development services tailored to meet your specific business needs</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8 mb-16">
                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Custom Web Development</h3>
                    <p class="text-gray-600 mb-6">We create responsive, scalable, and user-friendly websites using modern frameworks like React, Vue, and Angular.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Responsive Design
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            SEO Optimization
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            E-commerce Solutions
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>

                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-mobile"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Mobile App Development</h3>
                    <p class="text-gray-600 mb-6">Native and cross-platform mobile applications built with Flutter, React Native, and Swift for optimal performance.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            iOS & Android Development
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Cross-Platform Solutions
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            App Store Deployment
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>

                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-database"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Backend Development</h3>
                    <p class="text-gray-600 mb-6">Robust server-side solutions using Node.js, Python, Java, and cloud technologies for scalable applications.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            API Development
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Database Design
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Cloud Integration
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>

                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">UI/UX Design</h3>
                    <p class="text-gray-600 mb-6">User-centered design solutions that create intuitive and engaging experiences for your customers.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Wireframing & Prototyping
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            User Research
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Design Systems
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>

                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-cloud"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Cloud Solutions</h3>
                    <p class="text-gray-600 mb-6">Cloud infrastructure setup, migration, and management using AWS, Azure, and Google Cloud Platform.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Cloud Migration
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Serverless Architecture
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            DevOps & CI/CD
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>

                <div class="service-card bg-white p-8 rounded-lg shadow-md">
                    <div class="text-blue-600 text-4xl mb-6">
                        <i class="fas fa-headset"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Maintenance & Support</h3>
                    <p class="text-gray-600 mb-6">Ongoing maintenance, updates, and technical support to keep your applications running smoothly.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Regular Updates
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            Bug Fixing
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check text-green-500 mr-2"></i>
                            24/7 Monitoring
                        </li>
                    </ul>
                    <button onclick="showPage('contact')" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors">
                        Get Quote
                    </button>
                </div>
            </div>

            <div class="bg-blue-50 rounded-lg p-8 text-center">
                <h2 class="text-2xl font-semibold mb-4">Don't See What You Need?</h2>
                <p class="text-gray-600 mb-6">We specialize in custom solutions. Tell us about your project, and we'll create exactly what you need.</p>
                <button onclick="showPage('contact')" class="bg-blue-600 text-white px-8 py-3 rounded-lg hover:bg-blue-700 transition-colors">
                    Discuss Your Project
                </button>
            </div>
        </div>
    </section>

    <!-- About Page -->
    <section id="about" class="page-section pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="text-center mb-16">
                <h1 class="text-4xl font-bold text-gray-800 mb-4">About Bharatbinary</h1>
                <p class="text-gray-600 max-w-2xl mx-auto">Transforming ideas into exceptional digital experiences</p>
            </div>

            <div class="grid md:grid-cols-2 gap-12 items-center mb-16">
                <div>
                    <img src="https://placehold.co/600x400" alt="Modern software development team collaborating in a bright workspace with multiple monitors and whiteboards" class="rounded-lg shadow-xl" />
                </div>
                <div>
                    <h2 class="text-3xl font-semibold mb-6">Our Story</h2>
                    <p class="text-gray-600 mb-6">
                        Bharatbinary was founded with a simple mission: to deliver high-quality software solutions that empower businesses to thrive in the digital age. With years of experience in the industry, we've helped numerous clients transform their vision into reality.
                    </p>
                    <p class="text-gray-600 mb-6">
                        Our team consists of passionate developers, designers, and project managers who are dedicated to creating software that not only meets but exceeds expectations. We believe in building long-term relationships with our clients based on trust, transparency, and exceptional results.
                    </p>
                    <div class="grid grid-cols-2 gap-6">
                        <div class="flex items-center">
                            <div class="bg-blue-100 p-3 rounded-full mr-4">
                                <i class="fas fa-lightbulb text-blue-600 text-xl"></i>
                            </div>
                            <div>
                                <div class="font-semibold">Innovation</div>
                                <div class="text-sm text-gray-600">Cutting-edge solutions</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-blue-100 p-3 rounded-full mr-4">
                                <i class="fas fa-users text-blue-600 text-xl"></i>
                            </div>
                            <div>
                                <div class="font-semibold">Collaboration</div>
                                <div class="text-sm text-gray-600">Teamwork approach</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-blue-100 p-3 rounded-full mr-4">
                                <i class="fas fa-clock text-blue-600 text-xl"></i>
                            </div>
                            <div>
                                <div class="font-semibold">Timely Delivery</div>
                                <div class="text-sm text-gray-600">On-time projects</div>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="bg-blue-100 p-3 rounded-full mr-4">
                                <i class="fas fa-shield-alt text-blue-600 text-xl"></i>
                            </div>
                            <div>
                                <div class="font-semibold">Quality</div>
                                <div class="text-sm text-gray-600">Premium standards</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-gray-50 rounded-lg p-8 mb-16">
                <h2 class="text-3xl font-semibold text-center mb-8">Our Process</h2>
                <div class="grid md:grid-cols-4 gap-8">
                    <div class="text-center">
                        <div class="bg-blue-600 text-white w-12 h-12 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="font-bold text-xl">1</span>
                        </div>
                        <h3 class="font-semibold mb-2">Discovery</h3>
                        <p class="text-gray-600 text-sm">We start by understanding your requirements, goals, and vision for the project.</p>
                    </div>
                    <div class="text-center">
                        <div class="bg-blue-600 text-white w-12 h-12 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="font-bold text-xl">2</span>
                        </div>
                        <h3 class="font-semibold mb-2">Planning</h3>
                        <p class="text-gray-600 text-sm">We create a detailed project plan with timelines, milestones, and deliverables.</p>
                    </div>
                    <div class="text-center">
                        <div class="bg-blue-600 text-white w-12 h-12 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="font-bold text-xl">3</span>
                        </div>
                        <h3 class="font-semibold mb-2">Development</h3>
                        <p class="text-gray-600 text-sm">Our team builds your solution using agile methodologies and best practices.</p>
                    </div>
                    <div class="text-center">
                        <div class="bg-blue-600 text-white w-12 h-12 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="font-bold text-xl">4</span>
                        </div>
                        <h3 class="font-semibold mb-2">Delivery</h3>
                        <p class="text-gray-600 text-sm">We deploy your solution and provide ongoing support and maintenance.</p>
                    </div>
                </div>
            </div>

            <div class="text-center">
                <h2 class="text-3xl font-semibold mb-6">Ready to Start Your Project?</h2>
                <p class="text-gray-600 mb-8">Let's discuss your ideas and create something amazing together.</p>
                <button onclick="showPage('contact')" class="bg-blue-600 text-white px-8 py-3 rounded-lg hover:bg-blue-700 transition-colors">
                    Get in Touch
                </button>
            </div>
        </div>
    </section>

    <!-- Contact Page -->
    <section id="contact" class="page-section pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="text-center mb-16">
                <h1 class="text-4xl font-bold text-gray-800 mb-4">Get Your Project Quote</h1>
                <p class="text-gray-600 max-w-2xl mx-auto">Tell us about your project requirements, and we'll provide you with a detailed quote</p>
            </div>

            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <div class="bg-white rounded-lg shadow-md p-8">
                        <h2 class="text-2xl font-semibold mb-6">Project Details</h2>
                        <form id="projectForm" class="space-y-6">
                            <div>
                                <label class="block text-gray-700 mb-2">Project Type</label>
                                <select class="w-full p-3 border border-gray-300 rounded-lg form-input">
                                    <option value="">Select Project Type</option>
                                    <option value="website">Website Development</option>
                                    <option value="webapp">Web Application</option>
                                    <option value="mobile">Mobile App</option>
                                    <option value="custom">Custom Software</option>
                                    <option value="ecommerce">E-commerce Store</option>
                                    <option value="other">Other</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Project Description</label>
                                <textarea 
                                    placeholder="Describe your project in detail..." 
                                    class="w-full p-3 border border-gray-300 rounded-lg form-input h-32"
                                ></textarea>
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Features Required</label>
                                <div class="grid grid-cols-2 gap-3">
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">Responsive Design</span>
                                    </label>
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">User Authentication</span>
                                    </label>
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">Payment Integration</span>
                                    </label>
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">Admin Panel</span>
                                    </label>
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">Database</span>
                                    </label>
                                    <label class="flex items-center">
                                        <input type="checkbox" class="mr-2">
                                        <span class="text-gray-600">API Integration</span>
                                    </label>
                                </div>
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Timeline</label>
                                <select class="w-full p-3 border border-gray-300 rounded-lg form-input">
                                    <option value="">Select Timeline</option>
                                    <option value="urgent">Urgent (1-2 weeks)</option>
                                    <option value="fast">Fast (2-4 weeks)</option>
                                    <option value="standard">Standard (1-2 months)</option>
                                    <option value="flexible">Flexible (2+ months)</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Budget Range</label>
                                <select class="w-full p-3 border border-gray-300 rounded-lg form-input">
                                    <option value="">Select Budget Range</option>
                                    <option value="under-1k">Under $1,000</option>
                                    <option value="1k-5k">$1,000 - $5,000</option>
                                    <option value="5k-10k">$5,000 - $10,000</option>
                                    <option value="10k-25k">$10,000 - $25,000</option>
                                    <option value="25k+">$25,000+</option>
                                </select>
                            </div>
                        </form>
                    </div>
                </div>

                <div>
                    <div class="bg-white rounded-lg shadow-md p-8">
                        <h2 class="text-2xl font-semibold mb-6">Your Information</h2>
                        <form class="space-y-6">
                            <div>
                                <label class="block text-gray-700 mb-2">Full Name</label>
                                <input type="text" placeholder="Your full name" class="w-full p-3 border border-gray-300 rounded-lg form-input">
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Email Address</label>
                                <input type="email" placeholder="your@email.com" class="w-full p-3 border border-gray-300 rounded-lg form-input">
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Phone Number</label>
                                <input type="tel" placeholder="+1 (555) 000-0000" class="w-full p-3 border border-gray-300 rounded-lg form-input">
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Company Name</label>
                                <input type="text" placeholder="Your company name" class="w-full p-3 border border-gray-300 rounded-lg form-input">
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">How did you hear about us?</label>
                                <select class="w-full p-3 border border-gray-300 rounded-lg form-input">
                                    <option value="">Select option</option>
                                    <option value="google">Google Search</option>
                                    <option value="referral">Referral</option>
                                    <option value="social">Social Media</option>
                                    <option value="other">Other</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-gray-700 mb-2">Additional Notes</label>
                                <textarea 
                                    placeholder="Any additional information or specific requirements..." 
                                    class="w-full p-3 border border-gray-300 rounded-lg form-input h-24"
                                ></textarea>
                            </div>

                            <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700 transition-colors font-semibold">
                                Submit Quote Request
                            </button>
                        </form>
                    </div>

                    <div class="bg-blue-50 rounded-lg p-6 mt-8">
                        <h3 class="font-semibold mb-4">What happens next?</h3>
                        <ul class="space-y-2 text-sm text-gray-600">
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                                <span>We'll review your requirements within 24 hours</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                                <span>Schedule a free consultation call to discuss details</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                                <span>Receive a detailed project proposal and quote</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                                <span>Start your project with zero commitment</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Bharatbinary</h3>
                    <p class="text-gray-400 mb-4">Transforming ideas into exceptional digital experiences.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white">
                            <i class="fab fa-github"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Services</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Web Development</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Mobile Apps</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Custom Software</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">UI/UX Design</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Company</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Our Process</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Case Studies</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Blog</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-semibold mb-4">Contact</h4>
                    <ul class="space-y-2">
                        <li class="flex items-start">
                            <i class="fas fa-envelope text-gray-400 mt-1 mr-2"></i>
                            <span class="text-gray-400">info@bharatbinary.com</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-phone text-gray-400 mt-1 mr-2"></i>
                            <span class="text-gray-400">+1 (555) 123-4567</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt text-gray-400 mt-1 mr-2"></i>
                            <span class="text-gray-400">123 Tech Street, Digital City</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2024 Bharatbinary. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Page navigation
        function showPage(pageId) {
            // Hide all pages
            document.querySelectorAll('.page-section').forEach(section => {
                section.classList.remove('active');
            });
            
            // Show selected page
            document.getElementById(pageId).classList.add('active');
            
            // Update navigation active state
            document.querySelectorAll('button').forEach(btn => {
                btn.classList.remove('nav-active');
            });
            
            // Find and activate current nav button
            const navButtons = document.querySelectorAll('button');
            navButtons.forEach(btn => {
                if (btn.textContent.toLowerCase().includes(pageId) || 
                    (pageId === 'home' && btn.textContent === 'Home')) {
                    btn.classList.add('nav-active');
                }
            });
            
            // Scroll to top
            window.scrollTo(0, 0);
        }

        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Form submission
        document.querySelectorAll('form').forEach(form => {
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Thank you for your submission! We will contact you within 24 hours.');
                this.reset();
            });
        });

        // Close mobile menu when clicking outside
        document.addEventListener('click', function(e) {
            const menu = document.getElementById('mobile-menu');
            const menuButton = document.getElementById('mobile-menu-button');
            
            if (!menu.contains(e.target) && !menuButton.contains(e.target) && !menu.classList.contains('hidden')) {
                menu.classList.add('hidden');
            }
        });
    </script>
</body>
</html>

    

