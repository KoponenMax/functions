# functions

1)Перепишите функцию, используя оператор '?' или '||'
Следующая функция возвращает true, если параметр age больше 18.
В ином случае она задаёт вопрос confirm и возвращает его результат.

function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    return confirm('Родители разрешили?');
  }
}


function checkAge(age) {
	return (age > 18) ? true : confirm('Родители разрешили?');
}



2) Напишите функцию min(a,b), которая возвращает меньшее из чисел a и b.

function min(a,b){
	if (a < b){
		return alert (a);
	}
	else if (a == b){
		return alert ('Они равны');
	}
	else return alert (b);
}


3)Замените код Function Expression стрелочной функцией:

 function ask(question, yes, no) {
  if (confirm(question)) yes()
  else no();
}
ask(
  "Вы согласны?",
  function() { alert("Вы согласились."); },
  function() { alert("Вы отменили выполнение."); }
);



let ask = (question, yes, no) => (confirm(question))? yes() : no ();
ask("solasni??", () => alert("Da"), () => alert("otmena")); 



4) Напишите функцию, которая принимает строку и букву,которую необходимо найти, в качестве аргументов , и возвращает количество символов char , содержащихся в строке

function countChar(str, char){
  let count = '';
  
  for (N = 0; N < str.length; N++){
    if (str.charAt(N) == char){
      count = count + char;
        }
   }
    return count.length;  
}
