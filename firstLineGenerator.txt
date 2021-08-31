//The first line generator randomly creates the first sentence of a story.

//The phraseMaker object stores the diferent pieces of information.
let phraseMaker = {
    time: ['Once upon a time', 'It happened in a distant future', 'Not long ago', 'Before you were born'],
    place: [' in a remote country,', ' inside an apple,',' in a planet very similar to our own,',' ,nearby and old, abandoned castle,'],
    situation: [' two remarcable creatures were locked up in a lively discussion.', ' terrible events were about to take place.',' a boy was born.',
    ' there came to be something that would forever change everything.']
}

let getRandInt = max =>{
    return Math.floor(Math.random(max) * 4);
}

const firstLineGenerator = () =>{
    console.log( phraseMaker.time[getRandInt()] + phraseMaker.place[getRandInt()] + phraseMaker.situation[getRandInt()]);
}