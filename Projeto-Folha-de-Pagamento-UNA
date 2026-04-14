import java.util.ArrayList;
import java.util.Scanner;

abstract class Funcionario{
    protected String nome;
    protected int matricula;
    protected double salario = 2000;

    public Funcionario(String nome, int matricula, double salario){
        this.nome = nome;
        this.matricula = matricula;
        this.salario = salario;
    }
    
    public abstract double calcularSalario();
    public abstract String getTipo();
       
    public String toString(){
        return "Nome: " + nome +
        " | Tipo: "+ getTipo() +
        " | Matricula: " + matricula + 
        " | Salario: " + calcularSalario();
    }
}

class FuncionarioPadrao extends Funcionario{
    public FuncionarioPadrao(String nome, int matricula){
        super(nome, matricula, 2000); // 2000 = Salario
    }

    public double calcularSalario(){
    return salario;
    }

    public String getTipo(){
        return "Funcionario Padrão";
    }
}

class FuncionarioComissionado extends Funcionario{
    double valorDasVendas;
    int percentual;

    public FuncionarioComissionado(String nome, int matricula, double valorDasVendas, int percentual){
        super(nome, matricula, 2000);
        this.valorDasVendas = valorDasVendas;
        this.percentual = percentual;
    }

    public double calcularSalario(){
        return (valorDasVendas*percentual/100) + salario;
    }

    public String getTipo(){
        return "Funcionario Comissionado";
    }

}

class FuncionarioProducao extends Funcionario{
    int quantidadeDePecas;
    double valorDasPecas;

    public FuncionarioProducao(String nome, int matricula, int quantidadeDePecas, double valorDasPecas){
        super(nome, matricula, 2000);
        this.quantidadeDePecas = quantidadeDePecas;
        this.valorDasPecas = valorDasPecas;
        }

        public double calcularSalario(){
            return (valorDasPecas*quantidadeDePecas) + salario;
        }

        public String getTipo(){
            return "Funcionario Prdodução";
        }

    }

public class FolhaDePagamento {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<Object> lista = new ArrayList<>();

        int opcao;
        do{
            System.out.println("=== Folha de pagamento ===");
            System.out.println("1. Cadastrar funcionario padrão");
            System.out.println("2. Cadastrar funcionario comissionado");
            System.out.println("3. Cadastrar funcionario produção");
            System.out.println("0. Sair do programa");
            System.err.print("\nDigite a sua opção: ");
            opcao = scanner.nextInt();
            scanner.nextLine();

            switch (opcao) {
                case 1:
                    System.out.print("\nDigite o nome do funcionario: ");
                    String nome = scanner.nextLine();

                    System.out.print("Digite a matricula do funcionario: ");
                    int matricula = scanner.nextInt();
                    scanner.nextLine();

                    FuncionarioPadrao p = new FuncionarioPadrao(nome, matricula);
                    lista.add(p);
                    System.out.println("\nFuncionario cadastrado com sucesso!" + "\n" );
                    break;
            
                case 2:
                    System.out.print("\nDigite o nome do funcionario: ");
                    String nome2 = scanner.nextLine();

                    System.out.print("Digite a matricula do funcionario: ");
                    int matricula2 = scanner.nextInt();

                    System.out.print("Digite o valor das vendas: ");
                    double valorDasVendas = scanner.nextDouble();

                    System.out.print("Digite o percentual: ");
                    int percentual = scanner.nextInt();

                    FuncionarioComissionado p2 = new FuncionarioComissionado(nome2, matricula2, valorDasVendas, percentual);
                    lista.add(p2);
                    System.out.println("\nFuncionario cadastrado com sucesso!" + "\n");
                    break;
                    
                case 3:
                    System.out.print("\nDigite o nome do funcionario: ");
                    String nome3 = scanner.nextLine();

                    System.out.print("Digite a matricula do funcionario: ");
                    int matricula3 = scanner.nextInt();

                    System.out.print("Digite a quantidade de peças: ");
                    int quantidadeDePecas = scanner.nextInt();

                    System.out.print("Digite o valor das Peças: ");
                    double valorDasPecas = scanner.nextDouble();

                    FuncionarioProducao p3 = new FuncionarioProducao(nome3, matricula3, quantidadeDePecas, valorDasPecas);
                    lista.add(p3);
                    System.out.println("\nFuncionario cadastrado com sucesso !" + "\n");
                    break;

                case 0:
                    System.out.println("\nEncerrando o programa ...");
                
                    System.out.println("\n=== Lista de pessoas ===");
                    for (Object obj  : lista) {
                        
                        System.out.println(obj); 
                    }
                        System.out.println("\nQuantidade de pessoas cadastradas: " + lista.size() + "\n");
                

                        break;
                
                default:
                    System.out.println("\nOpção Invalida\n");
                    break;
            }


        } while (opcao != 0);
        
    }

}
