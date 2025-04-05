// Employee.java
class Employee {
    String name;
    double baseSalary;

    // Constructor
    Employee(String name, double baseSalary) {
        this.name = name;
        this.baseSalary = baseSalary;
    }

    // Method to calculate salary (to be overridden)
    double calculateSalary() {
        return baseSalary;
    }
}

// Manager.java
class Manager extends Employee {
    double bonus;

    // Constructor
    Manager(String name, double baseSalary, double bonus) {
        super(name, baseSalary);
        this.bonus = bonus;
    }

    // Overridden method
    @Override
    double calculateSalary() {
        return baseSalary + bonus;
    }
}

// Programmer.java
class Programmer extends Employee {
    double overtime;

    // Constructor
    Programmer(String name, double baseSalary, double overtime) {
        super(name, baseSalary);
        this.overtime = overtime;
    }

    // Overridden method
    @Override
    double calculateSalary() {
        return baseSalary + overtime;
    }
}

// Main.java
public class Main {
    public static void main(String[] args) {
        Manager m1 = new Manager("Alice", 70000, 10000);
        Programmer p1 = new Programmer("Bob", 50000, 5000);

        System.out.println("Manager Salary for " + m1.name + ": $" + m1.calculateSalary());
        System.out.println("Programmer Salary for " + p1.name + ": $" + p1.calculateSalary());
    }
}
