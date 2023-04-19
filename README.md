# min-max-index-



//To find min and max numbers in an array and accessing from the method, declaration in main method and passing method.

class Array {

    void method(int max, int min, int indexmax, int indexmin){

        System.out.println(" The maximum number in the array is : "+ max+ " ,"+ indexmax);

        System.out.println(" The minimum number in the array is : "+min+ " ,"+ indexmin);

    }

    public static void main(String... test) {

        int a[]=new int[10];

        a=new int[]{1,2,3,44,443};

        int max = a[0]; int min=a[0]; int indexmax=0; int indexmin=0;

        for(int i=0;i<a.length;i++){

            if(a[i]>max){

                max=a[i];

                indexmax=i;

            }

            else if(a[i]<max){

                min=a[i];

                indexmin=i;

            }

        }

        Array arr=new Array();

        arr.method(max,min,indexmax,indexmin);

    }

}

/*

 The maximum number in the array is : 443 ,4

 The minimum number in the array is : 1 ,0

 */
