**********FUNÇÕES NATIVAS PARA STRING**********

1. Remover espaços de um string;

````
trim();

````
2. Transformar toda em minúscula ou maíuscula:

````
strtolower($name)."<br>";
strtoupper($name)."<br>";

````

3. Transformar apenas a primeira letra em caia alta:

````
ucfirst($name)."<br>";

````

4. Transformar uma palavra por outra;

````
echo str_replace("Lima", "Póvoa", $name)."<br>";

// Ou seja, procure por "Lima", Substitua por "Póvoa" em $name;

````

5. Transformar uma plavra em invertida:

````
<?php
$name = "Gabriel Lima";

$replacedName = strrev($name);

echo "REPLACED NAME: ". $replacedName;
````

6. Pega apenas uma parte de nossa string:

****NOTE****
    - Se inserirmos o valor negativo, ele irá começar da direita para a esquerda.

````
<?php
$FullName = "Gabriel Lima";

$name = substr($FullName, 0, 5);

echo "NAME: ". $name;

````
7. Procurar uma palavra dentro de outra string:

````
$FullName = "Gabriel Lima";

$position = strpos($FullName, "l");

echo "NAME: ". $position;

//Ele retorna a posição onde aparece a primeira letra ou palavra a ser buscada

````

8. Transformar a primeira letra de cada palavra em caixa alta:

````
ucwords($string)
````

9. Transformar cada palavra de uma frase em um array:

````
<?php
$FullName = "joão gabriel de lima póvoa";

$names = explode(" ", $FullName);

print_r($names);
````

10. Formatar número;

````
<?php
$number = 12913.12;

echo number_format($number,1,',');

// Primeiro parâmetro: variável;
// Quantidade de casas depois do ponto;
// Simbolo para sepaar os decimais com vírgula ou ponto
// simbolo para separar os milhares


**********"BR FORMAT: "**********

<?php
$number = 12913.12;

echo number_format($number,2,',', '.');

*********************************
````

***********************************************