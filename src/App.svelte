<script>
  //All varibles that connect the HTML to Javascript
  let name = ''
  let form = ''
  let response = ''
  let response1 = ''
  let response2 = ''
  let response3 = ''
  let response4 = ''
  let response5 = ''
  let response6 = ''
  let response7 = ''
  let response8 = ''
  let response9 = ''
  let response10 = ''
  let points = 0
  let result = ''
  let result1 = ''
  let result2 = ''
  let result3 = ''
  let result4= ''
  let result5= ''
  let result6= ''
  let result7= ''
  let result8= ''
  let result9= ''
  let result10= ''
  
  function check(response) {
    // if the value of the answer includes the word yes then the result is correct and add one point if it includes no then the result is wrong
    if (response.includes('yes')) {
    result = 'correct'
    points += 1
    } else if (response.includes('no')) {
    result = 'wrong'
    } 



    if(response.includes ('Q1')){
      result1 = result
    }else if(response.includes ('Q2')){
      result2 = result
    }else if(response.includes ('Q3')){
      result3 = result
    }else if(response.includes ('Q4')){
      result4 = result
    }else if(response.includes ('Q5')){
      result5 = result
    }else if(response.includes ('Q6')){
      result6 = result
    }else if(response.includes ('Q7')){
      result7 = result
    }else if(response.includes ('Q9')){
      result9 = result
    }else if(response.includes ('Q10')){
      result10 = result
    }
}
  

  function check2(){
    if (response8 === 'storm'){
    result8 = 'correct'
    points += 1
    } else {
    result8 = 'wrong'
    } 

    
    
  }
</script>
 
<label>
  Name: 
  <input bind:value={name}>
  Class: 
  <input bind:value={form}>
</label>

<h1>Welcome {name} from class {form} to the Marvel quiz</h1>

<h1>Quiz </h1>
 
  Q1 -   What is Black Widow's original name?
  <label>
    	"Marina Duyunova"

    <input type="radio" bind:group={response1} value={'Q1no1'}>
  </label>
  
  <label>
  	"Gregovich Kuznetsov"

    <input type="radio" bind:group={response1} value={'Q1no2'}>
  </label>
  
  <label>
  	"Natasha Romanova"

    <input type="radio" bind:group={response1} value={'Q1yes'}>
  </label>
  
  <button on:click={check(response1)}> Check </button>
 
  <p>
   {result1}
  </p>
 
<!-- <p>
  {points} points in total
</p> -->

  Q2 -     What is the thing on Tony Stark's chest called?

  <label>
    		"Core Reactor"

    <input type="radio" bind:group={response2} value={'Q2no3'}>
  </label>

  <label>
	  "Arc Reactor"
    <input type="radio" bind:group={response2} value={'Q2yes1'}>
  </label>
  
  <label>
      "Heart"
    <input type="radio" bind:group={response2} value={'Q2no4'}>
  </label>
  
  <button on:click={check(response2)}> Check </button>
 
  <p>
   {result2}
  </p>

  Q3 -  "In what movie did spiderman meet Tony Stark"

  <label>
    		"Advengers 1"

    <input type="radio" bind:group={response3} value={'Q3no3'}>
  </label>

  <label>
	  "Iron Man 3"
    <input type="radio" bind:group={response3} value={'Q3no1'}>
  </label>
  
  <label>
      "Captian America Civil War"
    <input type="radio" bind:group={response3} value={'Q3yes4'}>
  </label>
  
  <button on:click={check(response3)}> Check </button>
 
  <p>
   {result3}
  </p>

  Q4 -  "What is the real name of the Scarlet Witch?"

  <label>
    		"Marina Duyunova"

    <input type="radio" bind:group={response4} value={'Q4no3'}>
  </label>

  <label>
	  "Wanda Maximoff"
    <input type="radio" bind:group={response4} value={'Q4yes1'}>
  </label>
  
  <label>
      "Natasha Romanova"
    <input type="radio" bind:group={response4} value={'Q4no4'}>
  </label>
  
  <button on:click={check(response4)}> Check </button>
 
  <p>
   {result4}
  </p>

  Q5 -  "Which of the infinity stones is hidden on Vormir?"

  <label>
    		"Soul"

    <input type="radio" bind:group={response5} value={'Q5yes3'}>
  </label>

  <label>
	  "Mind"
    <input type="radio" bind:group={response5} value={'Q5no1'}>
  </label>
  
  <label>
      "Time"
    <input type="radio" bind:group={response5} value={'Q5no4'}>
  </label>
  
  <button on:click={check(response5)}> Check </button>
 
  <p>
   {result5}
  </p>

    Q6 -  "What is the name of the organisation which is revealed to have infiltrated S.H.I.E.L.D. in Captain America: The Winter Soldier?"

  <label>
    		"H.y.d.r.a"

    <input type="radio" bind:group={response6} value={'Q6yes3'}>
  </label>

  <label>
	  "S.W.O.R.D"
    <input type="radio" bind:group={response6} value={'Q6no1'}>
  </label>
  
  <label>
      "no one infiltrated sheild"
    <input type="radio" bind:group={response6} value={'Q6no4'}>
  </label>
  
  <button on:click={check(response6)}> Check </button>
 
  <p>
   {result6}
  </p>

  Q7 -  "In which film do we finally learn the backstory behind how Nick Fury lost his eye?"

  <label>
    		"Captain America: The Winter Soldier"

    <input type="radio" bind:group={response7} value={'Q7no3'}>
  </label>

  <label>
	  "Captain Marvel"
    <input type="radio" bind:group={response7} value={'Q7yes1'}>
  </label>
  
  <label>
      "Captain America: The First Advenger"
    <input type="radio" bind:group={response7} value={'Q7no4'}>
  </label>
  
  <button on:click={check(response7)}> Check </button>
 
  <p>
   {result7}
  </p>

  Q8 -  "What is the name of the axe created for and then used by Thor in Avengers: Infinity War?"

  <label>
    <input type="text" bind:value={response8}>
  </label>
  
  <button on:click={check2(response8)}> Check </button>
 
  <p>
   {result8}
  </p>


 
<p>
  {points} points in total
</p>