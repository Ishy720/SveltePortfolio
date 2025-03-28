<section id="timeline" class="timeline-container">
    <div class="timeline-info">
        <h2>My Timeline</h2>
        <div class="timeline">
            <div class="timeline-item left">
                <div class="content">
                    <h3>2024 - Now</h3>
                    <p>Began my journey as a Junior Software Engineer at Total Merchandise.</p>
                </div>
            </div>
            <div class="timeline-item right">
                <div class="content">
                    <h3>2023</h3>
                    <p>Graduated with a First Class Honours in Computer Science, achieving a <strong>4.25 GPA</strong> at 20 years old.</p>
                </div>
            </div>
            <div class="timeline-item left">
                <div class="content">
                    <h3>2022</h3>
                    <p>Worked as a Web Development teaching assistant at the University of East Anglia (UEA).</p>
                </div>
            </div>
            <div class="timeline-item right">
                <div class="content">
                    <h3>2020</h3>
                    <p>Turned 18 and started my studies at the University of East Anglia (UEA).</p>
                </div>
            </div>
            <div class="timeline-item left">
                <div class="content">
                    <h3>2018-2020</h3>
                    <p>Studied A-Levels at Suffolk One College. Achieved an AAB in Mathematics, Electronics and Computer Science.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<style>
       .timeline-container {
        display: flex;
        flex-direction: column;
        color: white;
        height: fit-content;
        width: 100%;

        .timeline-info {
            display: flex;
            height: fit-content;
            margin: clamp(5px, 5vw, 60px);
            font-size: clamp(1rem, 1.5vw, 2rem);
            flex-direction: column;
        }

        .timeline {
            position: relative;
            max-width: 900px;
            margin: 50px auto;
        }

        .timeline::after {
            content: '';
            position: absolute;
            width: 5px;
            background-color: white;
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -3px;
        }
    
        .timeline-item {
            position: relative;
            width: 50%;
            padding: 10px 20px;
            box-sizing: border-box;
        }
    
        .timeline-item.left {
            left: 0;
            text-align: right;
            margin-left: -15px;
        }
    
        .timeline-item.right {
            left: 50%;
            margin-left: 15px;
            text-align: left;
        }
    
        .timeline-item .content {
            padding: 20px;
            background: #fcaa67;
            border-radius: 15px;
            position: relative;
        }
    
        .timeline-item.left .content::after,
        .timeline-item.right .content::after {
            content: '';
            position: absolute;
            top: 15px;
            width: 0;
            height: 0;
            border-style: solid;
        }
    
        .timeline-item.left .content::after {
            right: -10px;
            border-width: 5px 0 5px 10px;
            border-color: transparent transparent transparent #fcaa67;
        }
    
        .timeline-item.right .content::after {
            left: -10px;
            border-width: 5px 10px 5px 0;
            border-color: transparent #fcaa67 transparent transparent;
        }
        
        .timeline-item::before {
            content: '';
            position: absolute;
            top: 20px;
            width: 20px;
            height: 20px;
            background: #fcaa67;
            border-radius: 50%;
            z-index: 999;
        }
    
        .timeline-item.left::before {
            right: -25px;
        }
    
        .timeline-item.right::before {
            left: -25px;
        }
    }

</style>
