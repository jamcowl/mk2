<template>
  <section>
    <div class="container">
      <div class="item">
        <h1>FAQ.</h1>
      </div>

      <div class="item" v-for="i in faqs">
        <h3>{{ i.question }}</h3>
        <p v-html="i.answer" />
      </div>

      <div class="item">
        <h3>Got anything else?</h3>
        <p>
          Contact us by <a href="mailto:contact@hacksurrey.uk">email</a>,
          ping us on <a href="https://facebook.com/hacksurrey">Facebook</a>,
          or shoot us a <a href="https://twitter.com/hacksurrey">tweet</a>.
          We'll get back to you as soon as possible!
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
        faqs: [
          {question: 'What exactly is this?', answer: 'HackSurrey Mk2 is a Hackathon at the University of Surrey: 150 students, 24 hours, what will <b>you</b> build?'},
          {question: 'Are tickets free?', answer: `Of course they are! Thanks to our lovely sponsors, HackSurrey Mk2 tickets are absolutely free!`},
          {question: 'What is a hackathon?', answer: 'A hackathon is best described as an "invention marathon". Anyone who has an interest in technology attends a hackathon to learn, build, and share their creations over the course of a weekend in a relaxed and welcoming atmosphere. You don’t have to be a programmer and you certainly don’t have to be majoring in Computer Science.'},
          {question: 'But when and where?', answer: 'HackSurrey Mk2 will take place on the 9th and 10th of February 2019 at the <a href="https://goo.gl/maps/a85vhjCXA6K2">University of Surrey in Guildford</a>.'},
          {question: 'What should I bring?', answer: "You should bring your laptop, charger, and phone. You must not forget to bring your <strong>student ID</strong>, and lots of motivation. You'll be able to work overnight in the venue, so you might want to bring stuff like sleeping bags, toiletries, blanket, etc."},
          {question: `What if I can't code?`, answer: `Not a problem! Regardless of what you think of your technical ability, this will be a great opportunity to learn some new skills!`},
          {question: 'What about non-UK?', answer: 'You are still more than welcome to join us! However, you should know that we do not offer travel reimbursements.'},
          {question: 'How can I help?', answer: `<a href="mailto:contact@hacksurrey.uk">Be a Volunteer!</a> Volunteers can still participate and will receive extra goodies in exchange for their effort.`},
        ]
    }
  }
}
</script>

<style lang="sass" scoped>
section
  display: flex
  min-width: 96%
  padding: 1.5em 2em
  flex-direction: column

.container
  display: flex
  flex-wrap: wrap
  justify-content: space-around

.item
  margin: .5em
  flex: 1 1 auto
  padding: 1.5em
  flex-basis: 30%
  min-width: 300px
  border-radius: 2px
  break-inside: avoid-column
  h1
    padding: 0
    color: #FF3232
    font-size: 3.5em
    font-weight: 500
    margin: 0 0 5px 0
  h3
    padding: 0
    color: #FF3232
    font-weight: 100
    margin: 0 0 5px 0
    font-size: 1.75em
  p
    margin: 0
    color: #FF3232
    font-weight: 300
    text-align: justify

.item:last-child
  background-color: #FF3232
  a
    color: #ffffff
  h3, p
    color: #ffffff

strong
  text-decoration: underline
</style>
