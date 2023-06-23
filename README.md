# java creating person with name ,age,country
public class Main {
    public static void main(String[] args) {
        class person{
            private String name;
            private int age;
            private String country;

            public String getName() {
                return name;
            }

            public void setName(String name) {
                this.name = name;
            }

            public int getAge() {
                return age;
            }

            public void setAge(int age) {
                this.age = age;
            }

            public String getCountry() {
                return country;
            }

            public void setCountry(String country) {
                this.country = country;
            }
        }
        person myobj = new person();

        myobj.setName("aravind");
        myobj.setAge(Integer.parseInt("25"));
        myobj.setCountry("india");

        String name = myobj.getName();
        int age = myobj.getAge();
        String country = myobj.getCountry();

        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.print("Country " +country);
    }
}
