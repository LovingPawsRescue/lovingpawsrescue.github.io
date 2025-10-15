---
layout: default
title: "FAQs"
permalink: /faqs
---

<h1 style="text-align:center; margin-top: 2rem;">Frequently Asked Questions</h1>

<div style="max-width:800px; margin:2rem auto; padding:1rem;">

  <!-- FAQ Item -->
  <div class="faq-item">
    <button class="faq-question">How can I help?</button>
    <div class="faq-answer">
      <p>If you are not in a position to adopt, there are still plenty of other ways you can help us make a difference. We are always in need of more fosters             to help care for our animals until they find their forever home. If you are interested in fostering, please fill out 
        <a href="https://aivvlhly.formester.com/f/hyLNDHMDw" style="color:#3366cc; text-decoration:underline;">
          this form
        </a>
    </div>
  </div>
  
  <div class="faq-item">
    <button class="faq-question">How does the adoption process work?</button>
    <div class="faq-answer">
      <p>To start the adoption process, simply fill out [the adoption form](https://aivvlhly.formester.com/f/E3KbE110G). Once approved, we'll ask you to send a video of your home for a home check and proof of payment of the adoption fee. Once everything is finalised, your new dog or cat can go with you to their forever home.</p>
    </div>
  </div>

  <div class="faq-item">
    <button class="faq-question">How much is your adoption fee?</button>
    <div class="faq-answer">
      <p>Our adoption fee is R1300. This covers the dog or cat's first vaccinations, microchipping, sterilisation, deworming and tick treatments. If the animal           isn't 6 months old yet, we'll organise a free sterilisation at one of our vets when the puppy or kitten is old enough.</p>
    </div>
  </div>

  <div class="faq-item">
    <button class="faq-question">How can I donate?</button>
    <div class="faq-answer">
      <p>We have over 200 cats and dogs in our care, and appreciate all help, including donations. Please use [this link](https://drive.google.com/file/d/1gKN8j9sISq0ozdlRR3N_ogXYFOCXUDJL/view?fbclid=IwZXh0bgNhZW0CMTAAYnJpZBExS3RFdExHNEU0aW9QRm1GbQEeMQo-nziyyrksSrx-3S5uXhffUbm-8gb8hJcthiSM9RHIzEjYt9PN0_l2LCU_aem_H2r0jZbqomrSLxHkC_F5QA) to see how you can donate. </p>
    </div>
  </div>

  <div class="faq-item">
    <button class="faq-question">Who can I contact if I have other questions?</button>
    <div class="faq-answer">
      <p>If you have any other questions, please contact Nadia at 079 596 3336 or lovingpawsrescue11@gmail.com. </p>
    </div>
  </div>

</div>

<style>
.faq-item {
  border-bottom: 1px solid #ddd;
  margin-bottom: 1rem;
}

.faq-question {
  width: 100%;
  text-align: left;
  background: #f5f5f5;
  border: none;
  padding: 1rem;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  border-radius: 8px;
  transition: background 0.3s ease;
}

.faq-question:hover {
  background: #eaeaea;
}

.faq-answer {
  display: none;
  padding: 0.8rem 1rem;
  background: #fff;
  border-left: 4px solid #ccc;
  border-radius: 0 0 8px 8px;
}

.faq-answer p {
  margin: 0;
}

.faq-question.active {
  background: #dfe8ff;
}
</style>

<script>
const faqButtons = document.querySelectorAll(".faq-question");

faqButtons.forEach(btn => {
  btn.addEventListener("click", () => {
    const answer = btn.nextElementSibling;
    btn.classList.toggle("active");

    if (answer.style.display === "block") {
      answer.style.display = "none";
    } else {
      answer.style.display = "block";
    }
  });
});
</script>
