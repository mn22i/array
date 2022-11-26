# array

 static void Main(string[] args)
        {
            Console.WriteLine("Enter how many A person");
            int n=int.Parse(Console.ReadLine());
            Person[] arr = new Person[n];
            for(int i=0;i< n; i++)
            {
                arr[i] = new Person();
                Console.Write("Enter Person{0}Name", i + 1);
                arr[i].Getsetname = Console.ReadLine();
                Console.Write("Enter Person{0}Age", i + 1);
                arr[i].getsetage = int.Parse(Console.ReadLine());
            }
            Console.WriteLine("------Summary------");
            Person.DisplayInfo(arr);
            Console.WriteLine("------Summary after edit------");
            arr[0].Getsetname= "Amoni";
            Person.DisplayInfo(arr);
            Console.ReadLine();
        }
