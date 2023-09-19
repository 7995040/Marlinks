# Marlinks
O "Marlinlks HTML" será construído utilizando tecnologias web modernas, incluindo HTML5, CSS3 e JavaScript para o frontend. Além disso, podem ser usados frameworks e bibliotecas front-end, como Bootstrap ou Vue.js, para garantir um design elegante e uma experiência de usuário aprimorada. O servidor pode ser baseado em PHP, Node.js     


composer create-project --prefer-dist laravel/laravel nome-do-seu-projeto
cd nome-do-seu-projeto

php artisan make:model Pessoa -m

public function up()
{
    Schema::create('pessoas', function (Blueprint $table) {
        $table->id();
        $table->string('nome');
        $table->integer('idade');
        $table->string('sexo');
        $table->string('qualificacoes');
        $table->string('localizacao');
        $table->text('curriculo')->nullable();
        $table->timestamps();
    });
}
