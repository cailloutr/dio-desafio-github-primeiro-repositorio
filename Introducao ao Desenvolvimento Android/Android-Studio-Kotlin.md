# Manifest
- Informações essenciais para as ferramentas de compilação do Android, o Android SO, Google Play Store
- Recebe a declaração de todas as activities, permissões, etc
- Arquivo gerado e escrito em XML
- Declaração por tags (XML)

Package name = identificador unico (id do projeto)

# Activity
- Um dos componentes principais de um projeto Android
- Utiliza instancias dos métodos callback de ciclos de vida
- Pode corresponder a uma ou mais telas (fragments)
- Todas devem ser registradas/declarada do Android Manifest
- layout_activity.xml definie a exibição ao usuário
- Gerencia ciclos de vida, interações com o usuário, abertura de outras telas e aplicações, etc

# Ciclo de Vida
- Informa a criação, interrupção ou retomada de uma tela ou da destruição do processo pelo sistema/usuario
onCreate(), onStart(), onResume(), onPause(), onStop(), onDestroy()
- Ciclo Visível: ocorre enquanto o usuário esta com a aplicação aberta e tem retorno visual
- Ciclo Invisível: aplicação perde o foco, fora da visão do usuário

# Gradle is an open-source build automation tool that is designed to be flexible enough to build almost any type of software. 
- Configuração e automatização de build/compilação (processos internos do Android)
- build.gradle arquivo de consfiguração
- Gerencia importações, tipos de build, versão, etc
- Escrito em Groovy ou Kotlin DSL

# Layout
Jatpack compose - ui decorative (beta)
Layout XML - padrão
Viewbinding/databinding - arquivo de binding gerado a partir de todo o xml
 - LinearLayout: atributos em espectativa de lista vertical ou horizontal
 - Relative: tudo é relativo a outro item ou ao layout pai (a config do próprio elemento é prioridade ao layout pai) (permite sobreposição de elementos)
 - Constraint Layout: Restringir os compontentes aos limites do layout ou outro componente, focado em otimização. Substitui os demais layouts
 - FrameLayout - moldura, ideal para um único item

# Interação com a UI

 

# View
Todo compontente é uma view, herda da classe View

# Debbuging e Error Handeling
- Modo desenvolvedor: cria uma camada de teste e que proteje o celular durante cenários de teste
- Quando cira um projeto no android tem 2 buld types, debugging e o release (aplicação mais proximo do final): Habilitar debugging no build.gradle do modulo
- # ADB Android Debugging Bridge
- Conjunto de operações que facilita a manipulçação da aplicação no modo debugging em dispositivos físicos conectados a IDE
- Revogar/Fornecer permissões

# Logs
- DEBUG (Log.d)
- ERROR (Log.e)
- INFO (Log.i)
- VERBOSE (Log.v)
- WARNING (Log.w)

Primeiro parametro: TAG identificadora
Segundo parametro: mensagem informativa

# Erros e Exceptions
- ANRs - Aplicação não respondendo, falta de retorno a interação do usuário, blçoqueio da UI Thread. Dialog exibido pelo SO
- Throwable (Superclasse) - define prerrogativas para todos error e excptions que  serão emitidos pelo código
- Erros: cenário que pode ser evitado de maneira prévia. 
- Exception: geralmente quebram (crash) na aplicação 
- Thread.setuncaughtExceptionHandeler - tratar aq excpetion na thread
