Maksim Booga
My Contacts
Address: Georgia, Batumi
Phone: +9 591 038 726
E-mail: maksim.booga@gmail.com
About Me
I’m 16 years old. I studied computer science with a focus on web development HTML, CSS, JS, React so 

Skills
HTML
CSS
JavaScript (ES6+)
Git, GitHub
Photoshop, Figma
Code example
This is my solution for KATA from Codewars. We need to write the function “rndCode” generating random verification code in accordance with the following rules:

The code length should be 8.
The 1st and 2nd characters should be two uppercase letters. The range is “ABCDEFGHIJKLM”.
The 3rd-6th characters should be four numbers.
The 7th and 8th characters should be two symbols. The range is “~!@#$%^&*”.
Some valid verification code examples:

AB1234#$ MG6145$@ KJ2249@&
CD5678%^ IG7593~% FH8638@&
EF9012!@ GB7047%$ KD7604^%
function rndCode(){
  const char1_2="ABCDEFGHIJKLM";
  const char7_8="~!@#$%^&*";
  let generatedCode='';
  for (let i=0;i<8;i++) {
    if (i<2) {
      generatedCode+=char1_2[~~(char1_2.length*Math.random())];
    } else if (i>=2 && i<6) {
      generatedCode+=~~(9*Math.random());
    } else generatedCode+=char7_8[~~(char7_8.length*Math.random())];
  }
  return generatedCode;
}
console.log(rndCode());

Education
School

Languages
Belarussian - native
Ukranian - C1
Russian - C2
English - C1 according to IELTS
