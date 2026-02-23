# Krishanth (Kris) Suthaharan

I am an Electrical and Computer Engineer from the University of Toronto specializing in ASIC design, verification, and data/cloud systems, with industry experience at Intel, Synopsys and the Toronto Transit Commission (TTC). I hold a Bachelor's degree in Electrical & Computer Engineering from the University of Toronto with minors in Mechatronics/Robotics and Business, and I am currently pursuing a Master’s in ECE at the University of Toronto with emphasis in Data Analytics and Machine Learning.

## Technical Interests
- ASIC/FPGA Digital Design & Verification  
- Data Engineering & Cloud Infrastructure  
- Distributed Systems & Scalable Data Pipelines  
- Robotics & Software Systems  

## Leadership & Team Experience
I’ve been actively involved in multidisciplinary engineering teams at the University of Toronto:

- **Co-President**, Robotics for Space Exploration (RSX)  
- **Electrical Lead (2 years)**, RSX  
- **Junior Electrical Lead**, RSX  
- **Firmware Systems Division**, U of T Aerospace Team  

These roles strengthened my skills in technical leadership, cross-functional collaboration, and delivering complex engineering systems.

## What You'll Find Here
This GitHub showcases projects in:
- Data engineering pipelines & cloud analytics  
- Software engineering repos  
- Coding practice 
- and more!

## Let’s Connect
I’m always interested in collaborating on impactful engineering projects and discussing opportunities in ASIC design/verification, data engineering, and cloud infrastructure.

# Projects
Please note that the source code for some projects cannot be publicly released due to University of Toronto policies restricting the distribution of assignment solutions. To provide transparency, I have included detailed READMEs, architectural diagrams, and screenshots where possible to document design decisions, methodologies, and outcomes.

### Software Projects

#### Coinsight: Cryptocurrency Price Prediction | 2025
🔗 https://github.com/kris20012/crypto-price-prediction-rnn

• Implemented Elman RNN baseline and stacked LSTM with dropout & batch normalization achieving test accuracy of
68% to forecast next-day cryptocurrency prices using a sequence-to-one regression formulation and historical market data with a target relative error 10% or better
• Preprocessed 7.3M+ rows of OHLCV crypto data including handling missing timestamps, normalizing features, computing rolling statistics, cumulative returns, technical indicators (RSI, MACD, Bollinger Bands, OBV, ATR), and cyclical time encodings, increasing predictive signal by ∼25% for financial time series using 30-day sliding windows
• Designed and prepared training, validation, and test datasets with proper chronological splits, z-score scaling, and PyTorch DataLoaders
• Trained models with MAE loss & Adam optimizer, and visualized training/validation curves to monitor convergence, overfitting, and generalization

#### Cloud Inventory Management Platform | 2025
🔗 https://github.com/ThomasPazhaidam/Inventory-Management-System

• Designed a distributed inventory management system using Docker Swarm across two DigitalOcean nodes, enabling load-balanced API traffic with Traefik and real-time inventory synchronization via WebSockets and Redis Pub/Sub. <br />
• Provisioned a production-grade IaaS environment on DigitalOcean, configuring Linux VMs, Nginx, PostgreSQL, and REST integrations end-to-end while securing credentials with Docker Secrets. <br />
• Implemented JWT-based authentication and role-based access control enforcing least-privilege security. <br />
• Developed a fault-tolerant backup and recovery pipeline with automated PostgreSQL snapshots, restoring full database state in under 2 minutes and reducing potential data-loss risk by over 95%. <br />

#### Cloud Infrastructure Deployment | 2025
• Launched an Ubuntu 24.04 Droplet (1 vCPU, 1 GB RAM) using SSH key-based authentication and configured Nginx with PHP to deliver dynamic server-side content backed by PostgreSQL, achieving sub-200 ms response times. <br />
• Designed a PostgreSQL relational schema with role-based access control (www-data) ensuring 100% data persistence and secure access. <br />
• Automated IaaS validation by parsing JSON responses dynamically, reducing manual verification effort by approximately 80%. <br />

#### Containerized Task Management API | 2025
• Developed a RESTful API with 7 endpoints supporting full CRUD operations, partial updates, and deterministic state resets, returning 7 distinct HTTP status codes for robust client integration and automated testing with Postman. <br />
• Containerized and deployed the service to Fly.io using Docker, enforcing HTTPS and achieving reproducible builds across environments. <br />

#### Azure Cloud Diabetes Readmission Analytics | 2025
🔗 https://github.com/kris20012/Diabetes-Readmission-Risk-Analytics

• Engineered an end-to-end healthcare ETL pipeline ingesting a 100k+ record clinical dataset into ADLS via Azure Data Factory and Databricks, enabling scalable and reproducible analytics workflows. <br />
• Built batch ETL in Python to clean data, map ICD-9 codes into clinical categories, and normalize 50+ features, reducing data noise by ~20% and improving downstream model stability. <br />
• Implemented class balancing and feature engineering with cross-validated model evaluation; Random Forest improved F1-score by 13% over Logistic Regression, while Azure AutoML selected an XGBoost ensemble achieving 0.65 accuracy. <br />
• Developed a Power BI dashboard visualizing key readmission risk drivers using feature importance analysis, enabling data-driven clinical insights. <br />

#### Azure Cloud Workforce Insights | 2025
• Deployed an end-to-end Azure data platform, building an ADF ETL pipeline to ingest and transform workforce datasets from Blob Storage to Azure SQL DB with automated triggers every 3 minutes. <br />
• Configured cross-region ADLS Gen2 replication to provide geo-redundant storage for disaster recovery and compliance requirements. <br />
• Developed analytical SQL queries generating year-over-year workforce metrics across 10+ dimensions to support strategic workforce planning. <br />
• Built real-time staffing insights using Azure Stream Analytics, filtering and aggregating employment data with ~15-second latency for near-real-time monitoring. <br />

#### Distributed Recommender System on Apache Spark | 2025
• Designed a collaborative filtering recommender system using Spark MLlib on 1M+ movie ratings in Databricks, applying stratified train/test splits and cross-validated hyperparameter tuning to achieve 83% top-K accuracy. <br />
• Optimized Spark transformations through caching and partition tuning, reducing runtime by ~30% on large-scale aggregations. <br />
• Developed Spark SQL analytics pipelines to compute rating distributions and evaluate recommender performance, enabling data-driven tuning of recommendation quality. <br />

#### ETL Pipeline on Hadoop MapReduce | 2025
• Built a distributed data processing pipeline to ingest and analyze 10+ GB of numerical datasets in HDFS, enabling scalable batch analytics. <br />
• Optimized MapReduce performance using combiner-based aggregation, reducing network shuffle overhead by ~35% and improving job efficiency. <br />
• Implemented distributed k-means clustering with dynamic cluster sizing, automated centroid recalculation, and canopy clustering to reduce distance computations, improving convergence speed by 24%. <br />

#### Autonomous Farming Robot | 2024
•	Simplified plant incubation for busy people to enhance the nurturing process for healthy plants <br />
•	Developed livestreaming support for real-time camera feed to server using Java, ESP32 & Android Studio,  enabling users to monitor plants via an Android app <br />
•	Designed the electronics with a transformer, step-down regulators and fuses to deliver the correct power safely to all downstream devices <br />
•	Implemented serial (UART) communication between Arduino Uno and ESP32 to inform primary controller which plant to harvest <br />
•	Programmed the 3-axis gantry system using stepper motors with C++ & Arduino for precise movement to harvest plants
autonomously once they are detected to reach maturity via periodic scans using an ultrasonic sensor <br />
•	Achieved University of Toronto ECE Capstone Certificate of Distinction 

#### Autonomous Robot Search and Finding Objects | 2024
•	Implemented a SLAM algorithm in ROS using Gmapping and Rviz visualization software with C++ , ROS, TurtleBot, OpenCV to allow a TurtleBot
to traverse and explore a maze and generate a map of the environment (using graph theory) <br />
•	Programmed a node-based depth-first search algorithm to systematically explore unvisited areas <br />
•	Avoided obstacles by utilizing sensor data from laser and bumper sensors, backtracking to previous nodes <br />
•	Utilized the ROS AMCL and move_base packages to effectively navigate the robot to five objects placed at known locations on the map.
Tested algorithms using Gazebo simulation software. Gyroscope sensor data was used to calculate odometry data to gather positional and orientation measurements for efficient localization <br />
•	Used OpenCV framework to identify the objects in the FOV of an RGB camera using image recognition with SURF algorithm to detect features, 
FLANN algorithm to compare the object’s features to the template, and Lowe’s ratio test to filter good matches 

#### Brain	Tumour	MRI	Classification	Model |	2023
• Developed a	Convolutional	Neural	Network	(CNN)	machine	learning	(ML)	model	with Python that	successfully	classifies	brain
tumours	(abnormal	cell	developments	in	skull)	based	on	MRI	images	to	aid	medical	doctors	make	accurate	diagnosis <br />
• Collected	a	dataset	of	7500 images	with	Meningioma,	Pituitary,	Glioma	and	No	Tumour	pre-processing	the	images	with	
cv2	library	for	gray	scale,	histogram	equalization,	Gaussian	blur	(noise)	and	balancing	the	set	resizing	to	smallest	size <br />
• The	encoder	is	stacked	with	5	convolutional	layers	with	3x3	kernels	each	followed	by	ReLU	activation	function,	batch	
normalization and	max	pooling	to	extract	features	implemented	in	Python	with Pandas, Numpy	and	PyTorch	libraries <br />
• Flattened	the	feature	maps	from	the	last	convolutional	layer	into	a	2-layer	Artificial	Neural	Network	(ANN)	to	classify	
the	images	and	the	final	prediction	probabilities	are	determined	by	applying	a	SoftMax	function	for	the	distribution <br />
• Performing	hyperparameter	tuning,	achieved	a	model	with	94.4%	testing,	95.3%	validation	and 99.9%	training	
accuracy	beating	the	Random	Forest	Decision	Trees	algorithm	from	Scikit-learn	ML	library in	Python

#### Curriculus |	2022
🔗 https://github.com/ECE444-2022Fall/curriculus

• Developed	a	web	application using Python,	HTML/CSS,	ReactJS,	Flask,	Bootstrap	to	help	post-secondary	students	explore and	search courses	for	their	time	in	university,
create	a	course	plan	that	would	follow	the	requirements	to	become	an	engineer such	as	kernel,	depth	and	elective	
courses,	and	programmed	a	recursive	map	to	visually	see	course	prerequisites <br />
• Adopted	agile	development	practices	using	Jira.	<br />
• Developed	a	Flask	App	to	detect	if	a	snippet	of	text	is	Fake	News	or	not	using	machine	learning	(ML)	and	with Heroku	
to	make	the	model	accessible	as	a	service	using	a	REST	API	call. Deployed	the	ML	model	to	the	cloud	using	AWS	elastic	
beanstalk	for	ease	and	scalability,	and	measured	API	latency	over	100	calls	to	the	REST	server <br />
• Achieved	a	score	of	94%	(A+)	in	the	course and	4th place	out	of	a	class	of	about	120	students

#### Mapper: City Scout | 2021
•	Developed software application using C++ that would allow users to navigate through cities around the world in a user-friendly manner similar to Google Maps <br />
•	Added mouse hover functionality to aid users with how to use the software application, zooming and highlighting capabilities based on the user's search input, real-time search suggestions and autocompletion based on keyboard input from user, and pop-up message boxes for incorrect/successful user input operations and help button <br />
•	Implemented Libcurl functionality for users to view real-time delays on highway 401 and ability to view subway stations on the map <br />
•	Used a toggle button to show hidden second search bar to find path between two intersections. The path will be highlighted and have arrows for direction. <br />
The path determined by the application will be the shortest path implemented using Dijkstra’s Algorithm <br />
•	In order to solve the delivery truck problem with multiple pickups and dropoffs of packages, a greedy algorithm is implemented to determine the local best path optimizing the time by introducing a 2-D matrix to store the values to be reused and using 2-Opt Algorithm to change the delivery order to be efficient <br />
•	Used timers from Chrono Library to evaluate the speed of our program and boost its performance

<img width="737" alt="Screen Shot 2021-11-07 at 7 58 11 PM" src="https://user-images.githubusercontent.com/73756462/140669211-2f0e5762-5fbb-455e-b99e-44c108cb5993.png">

https://user-images.githubusercontent.com/73756462/140669510-139036ee-bf2c-4ef1-b259-6ca43d32d337.mov

<img width="751" alt="Screen Shot 2021-11-07 at 8 04 37 PM" src="https://user-images.githubusercontent.com/73756462/140669566-185c9db3-f369-42a9-827a-d0a2b875ed85.png">

https://user-images.githubusercontent.com/73756462/140669676-e09fb25e-4f67-4b5c-9eef-e0b7fc968310.mov

<img width="1248" alt="Screen Shot 2021-11-07 at 8 08 52 PM" src="https://user-images.githubusercontent.com/73756462/140669749-eb92c0fc-e605-4b63-b5d7-b3e145f69be0.png">
<img width="1238" alt="Screen Shot 2021-11-07 at 8 11 40 PM" src="https://user-images.githubusercontent.com/73756462/140669881-f3646f83-5a36-457c-8d67-f170b2416b28.png">
<img width="1234" alt="Screen Shot 2021-11-07 at 8 12 13 PM" src="https://user-images.githubusercontent.com/73756462/140669909-5db084ff-5960-4017-b65d-fb5ba442dad9.png">

<img width="1230" alt="Screen Shot 2021-11-07 at 8 13 12 PM" src="https://user-images.githubusercontent.com/73756462/140669970-10c836cc-8c77-458c-95f9-ca306b591496.png">

<img width="1105" alt="Screen Shot 2021-11-07 at 8 13 27 PM" src="https://user-images.githubusercontent.com/73756462/140669976-a6b4f0fc-7841-4818-8056-739ffd3f8e34.png">

https://user-images.githubusercontent.com/73756462/140670189-d7bbcccd-be10-4231-8b36-f84794260c76.mp4

#### Space: The Final Frontier | 2020

•	Developed software using C++ that would implement an artificial intelligence (AI) to destroy as many asteroids (randomly generated by a server) as possible to save the Starship Galaxy Explorer from destruction <br />
•	Designed an advanced linked list that observes asteroids in the ships vicinity and updates each asteroid in the list based on how it move in the x and y directions, it’s health after each shot by the ship and whether the asteroid is destroyed or moved away from the ship’s visible range <br />
•	The AI would traverse this list of asteroids and consider factors including proximity of asteroids to the ship, the reload time of each shot, the asteroids’ remaining health to decide on which asteroid to shoot at <br />
•	Once decided, the AI uses its method functionality to maneuver the ship controller by rotating the ship and firing a shot at the asteroid. All these operations repeat at every clock cycle of the CPU

#### Shape Generator Database | 2020

•	Developed software using C++ to allow users to store information about shapes in a memory (dynamic) efficient database  <br />
•	Designed a complex linked list with pointers to dynamically allocate and remove memory for each shape <br />
•	Implemented a command line with a graphical user interface for the user to ensure that there are no errors in the asserted commands and provided specific feedback as to what the particular error was parsed <br />
•	Inherited and reused code from others and extended the functionality (using object-oriented programming) to ensure that different shapes with different properties (information) can also be added to the database <br />
•	Created commands that allow users to create shapes, create shape subgroups, draw all or subgroups of shapes, move shapes from one subgroup to another, and remove shapes from the database by implementing methods in my linked list for efficient list traversal, list insertion, deletion of a node, and deep assignments

#### Reversi (Othello) | 2020

•	Developed software using C programming that would replicate the game of reverse to allow people to play the game at home during the COVID-19 pandemic; this method proved to be a quicker and cost-effective way of playing the game <br />
•	Programmed an artificial intelligence that can defeat human players using game trees, minimax algorithm and recursive implementation <br />
•	Ensured that the AI can make moves within one second of calculations allowing the program to be efficient <br />

#### Mastermind | 2019

•	Utilized Java to create the classical Mastermind game to make it easier and efficient to
play the game taking less time and it’s free. <br />
•	Implemented Graphical User Interface (GUI) for the game board and pins to make it 
visually appearing for the player

#### MP3 Player | 2018

•	Utilized Java to create an application that simulated an MP3 Player to allow customers
to listen to music of their preference <br />
•	Executed features including GUI for the menu, MP3 Player case design and selection 
of songs to make it user-friendly to navigate through and find songs efficiently

#### Chess | 2018

•	Developed software using Java that would replicate a traditional Chess game to be a more efficient
way of playing the game taking less time and no need for the physical board and pieces <br />
•	Added features including a virtual game board, menu and pieces lost for the GUI to make 
easier for the user to see and have a better experience

<br /><br />

### Hardware Projects

#### Optimized Processor | 2024

• Designed and implemented a 16-bit shared hardware processor on an Altera FPGA using Verilog/VHDL, modeling the control path as a finite state machine (FSM) and validating functionality with ModelSim simulations. <br />
• Improved throughput and performance by introducing pipeline register stages, analyzing latency vs. clock frequency trade-offs to optimize speed and power efficiency. <br />
• Engineered an FSM-driven control unit to manage register loading, ALU operations, and multiplexed datapath routing based on user-selected arithmetic functions. <br />
• Developed a 2D image convolution accelerator on FPGA and benchmarked performance against CPU and GPU implementations, demonstrating hardware acceleration benefits for parallel workloads. <br />
• Conducted timing, area, and power analysis for multi-clock designs, incorporating fixed-point and IEEE-754 floating-point representations to evaluate precision vs. resource utilization. <br />
• Implemented memory-mapped output registers and displayed computation results on LEDs and hexadecimal seven-segment displays for real-time user feedback. <br />

#### Music	Analyzer	|	2024
• Implemented a	live	trumpet	replicator	SoC	using System	Verilog,	C Programming on	the	Xilinx	Artix-7	(Nexys	4	DDR and	Video)	FPGA	boards collaborating
in	a	team	of	4 to	create	hardware	with	Vivado	(+IP	Integrator)	and software	on	the	MicroBlaze	processor	using	SDK <br />
• The	project	will	listen	to	audio	from	the	user	using	a	SPI	MEMS	microphone;	process	the	audio	data	in	real-time	using
digital	signal	processing	algorithms	that	include	sampling,	filtering,	equalization,	applying	the	Fast	Fourier	Transform
and	verification	with	MATLAB;	and	identify	the	note	being	played	by	determining	the	respective	frequency	(pitch) <br />
• The	positive	impact	of	the	project	will	be	with	learning	music	and	there	will	be	a	live	animated	trumpet	output	to	an
HDMI	monitor (from	FPGA).	This	graphical	interface	will	help	each	beginning	trumpeter see	how	to	play	a	music	piece

#### Operation | 2021
•	Implemented and embedded a computer system C Programming on the Intel® DE1-SoC board with ARM Cortex A9 processor to create a 
game that helps users learn about the various organs in the human body in an amusing manner <br />
•	Employed a combination of logic instructions, interrupts, registers, input/output devices including a keyboard, timer, <br />
7 Segment Displays, and VGA display to develop the software finite state machine for the game control

#### Logisim | 2020
•	Used Logisim (remote circuit development software) to implement 7400 series dual in-line package (DIP) chips to study circuits 
with logic gates and understand how they can be used to manipulate and produce signals as desired

#### Hexdecoder | 2020
•	Designed a hexdecoder circuit using Verilog with multiplexers, modular hierarchy, and a 7 segment display to display hexadecimal values according to four switch signals (four bits) <br />
•	Utilized Intel Quartus Prime to implement the Verilog design on FPGAs (Field Programmable Gate Array) describing the hexdecoder <br />
•	Simulated the hardware design using ModelSim software and verified the output waveforms to ensure that the tool synthesizes the circuit correctly the first time since it can be time consuming sometimes

#### Arithmetic Logic Unit (ALU) | 2020
•	Designed a 7-to-1 multiplexer using Verilog case statements in an always block <br />
•	Developed a ripple carry adder circuit that adds two 4-bit numbers using four instances of a full adder module <br />
•	Built and simulated an ALU by implementing all required operations including addition, subtraction, sign extension, etc., and connected the outputs to a 7-to-1 multiplexer  <br />
•	Using 3 select bits to drive the multiplexer select lines, the output value for the ALU can be chosen and then displayed on to LEDs and a set of HEX displays

#### Registers | 2020
•	Developed a gated D latch using Verilog that depends on the level of clock and placed two of them in series with opposite edges of clock to create an edge triggered D flip flop (also known as a primary-secondary flip flop) in which the output changes when the clock edge rises and also implemented an active low, synchronous reset <br />
•	Designed an 8-bit register by having 8 flip flops in parallel to one another <br />
•	Extended the functionality of the ALU by storing the output into an 8-bit register and implemented feedback into the second input of the ALU using the four least significant bits of the register output <br />
•	Designed and simulated a left/right 8-bit rotating register with parallel load using 8 instantiations of the flip flop module in which shift occurs by copying the bites to the next flip flop to the left or right on successive clock cycles. The parallel load enables the user to enter a preset set of 8 binary bits

#### Clocks and Counters | 2020
•	Implemented a series of 8 T-flip flops in series using Verilog with additional combinational logic to develop an 8-bit counter with an enable signal and an active low asynchronous reset <br />
•	Developed a rate divider (counter) that would use an industrial clock to increment a counter at varying speeds by having two counters. The rate divider creates pulses at the required rates by counting down certain numbers of clock cycles from the CPU clock frequency to achieve the desired speeds

#### Finite State Machines | 2020
•	Designed a finite state machine using Verilog that would identify certain sequences of binary patterns for the purpose of identifying specific numbers from a long sequence of binary bits <br />
•	Emulated a typical calculator by implementing a finite state machine for the control to load numbers entered by the user into registers. It also accounts for the wait state as the user clocks the information <br />
•	Used another separate finite state machine for the data path. Based on enables signals from the control path, the numbers entered by the user are stored in multiple registers. Then, it is relayed into Arithmetic Logic Units using multiplexers depending on the preferred arithmetic operation <br />
•	Finally, the output is stored in register and output to LEDs and Hexadecimal displays at run-time

#### Memory and VGA Display | 2020
•	Developed a RAM memory block using Quartus IP Catalog and Verilog to store the pixels in a frame buffer which is then used by the VGA Controller to display images on to a monitor <br />
•	Implemented a control finite state machine to take in user input and create enable signals for the data path <br />
•	Designed a finite state machine that would take X, Y and RGB colour inputs to develop squares on the screen by modulating counters to pixelate (4 x 4) 16 more squares going in a down-right direction

<br /><br />

### Circuit Design Projects

#### Arduino | 2017 – 2019

•	Using an Arduino UNO, programmed a police alarm independently with C++ to
detect when a thief would enter a room using a sensor and display a message on an 
LCD screen calling 911 while outputting a programmed police alarm <br />
•	Programmed a lighting system using Arduino and an Integrated Circuit chip to enable 
lights to turn on/off according to logical operators within the chip and binary systems <br />
•	Utilized Arduino to program a seven-segment display in C++ that would be able to simulate <br />
•	Timers such as the ones at Ice Hockey games to show time elapsed

#### Beetle Bot | 2017

•	Developed a device with SPDT (single pole double throw) switches, motors and other electrical 
components to create a device that would independently operate through a maze

#### Sumo Bot | 2018

•	Utilized Infrared Sensors and programming in C++ to maneuver a small robot that would
be used to stay in an arena, detect other Sumo Bots and engage in combat with them

# Contact

Email: krishanth.suthaharan@mail.utoronto.ca

LinkedIn: http://www.linkedin.com/in/krishanth-suthaharan

<!---
- 👋 Hi, I’m @kris20012
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
--->

<!---
kris20012/kris20012 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
