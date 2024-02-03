O [[Pytest]] é um framework de teste para Python que oferece uma abordagem feature-rich e baseada em plugins para testar código Python. Sua filosofia e recursos tornam a experiência de teste mais produtiva e agradável.

Em comparação com o módulo [[Unittest]] padrão do Python, o [[Pytest]] apresenta vantagens significativas. Ele permite que tarefas comuns sejam realizadas com menos código, promovendo uma abordagem mais concisa e expressiva.

### Características específicas

- **Sintaxe Concisa:** O [[Pytest]] utiliza uma sintaxe mais concisa para escrever testes, resultando em código mais limpo e legível.
- **[[Fixture]]:** O sistema de fixture do [[Pytest]] simplifica a configuração e limpeza de recursos necessários para testes.
- **Parametrização de Testes:** A capacidade de parametrizar testes facilmente ajuda a reduzir redundâncias e melhorar a manutenção.

### Modelo de testes padrão

A maioria dos testes funcionais segue o modelo **Arrange-Act-Assert**:
- Arrange - Organizar ou configurar as condições para o teste
- Act - Aja chamando alguma função ou método
- Assert - Afirme que alguma condição final é verdadeira

### **Funções e Módulos:**

- Mark
	- A funcionalidade de marcação pode nos ajudar a montar "tags" ou "grupos" para testes específicos. Podemos simplificar chamadas ou rodas testes específicos para casos específicos.
	- Exemplo:
	```python
	from pytest import mark
		  
		 @mark.tag
		 def test_meu_quinto_test():
			 assert True 
	```

### Comandos

- pytest
	- Executa todos os testes listados na pasta de testes.
- pytest -x 
	- Executa todos os testes com a condição de parada definida no primeiro teste que falhar.
- pytest --pdb {MUITO UTIL PRA DEBBUG}
	- Debbuger que mostra todo o escopo do teste que falhou
- pytest --junitxml report.xml
	- Salva um relatório em xml com o histórico de todos os testes rodados na suíte de testes.
- pytest -v: 
	- Mostra o nome dos testes executados
- pytest -s
	- Mostra as saídas no console
- pytest -k
	- Mostra a saída de testes no seguinte formato:
		- "nome_dos_testes": Filtra resultados

### Tipos de Output do Sistema

- test_file.py .  : Passou no testes
- test_file.py F : Falhou no testes
- test_file.py x : Falha esperada no testes
- test_file.py X : Falha esperada, mas não falhou no testes
- test_file.py s : Pulou (skiped) no testes

### **Integração com Projetos:**

- Analise a integração da biblioteca em projetos existentes.
- Entenda como os módulos da biblioteca podem ser incorporados de maneira eficiente.
### **Boas Práticas de Uso:**

- Estude as boas práticas recomendadas para o uso da biblioteca.
- Compreenda padrões de codificação e convenções que facilitam a manutenção e colaboração.

### **Compatibilidade e Dependências:**

 - O [[Pytest]] é altamente compatível com testes escritos usando [[Unittest]].
- Avalie a compatibilidade da biblioteca com diferentes versões da linguagem e outros frameworks.
- Analise as dependências e seus impactos no projeto.
###  **Documentação Detalhada:**

- Explore a documentação da biblioteca para compreender detalhes de implementação.
- Utilize exemplos práticos fornecidos na documentação para uma compreensão mais clara.
###  **Comunidade e Suporte:**

- Pesquise sobre a comunidade em torno da biblioteca.
- Avalie a atenção dada aos problemas, atualizações e suporte técnico.
###  **Casos de Uso Reais:**

- Estude casos de uso reais em que a biblioteca foi aplicada com sucesso.
- Analise implementações práticas e lições aprendidas por outros desenvolvedores.
###  **Atualizações e Novas Versões:**

- Mantenha-se atualizado sobre as atualizações e novas versões da biblioteca.
- Compreenda como as atualizações podem impactar o seu projeto e se há benefícios significativos.