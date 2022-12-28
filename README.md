import jdk.swing.interop.SwingInterOpUtils;

import java.util.ArrayList;
import java.util.Scanner;

public class EvenOrganiser {

    private String CUSTID;
    private String CUSTNAME;
    private String CUSTADDR;
    private String CUSTEMAIL;
    private String CUSTPHONE;

    public String getCUSTEMAIL(){
        return CUSTEMAIL;
    }
    public void setCUSTEMAIL(String CUSTEMAIL){
        this.CUSTEMAIL = CUSTEMAIL;
    }
    public void setCUSTADDR(String CUSTADDR){
        this.CUSTADDR = CUSTADDR;
    }
    public void setCUSTID(String CUSTID){
        this.CUSTID = CUSTID;
    }
    public void setCUSTNAME(String CUSTNAME){
        this.CUSTNAME = CUSTNAME;
    }
    public void setCUSTPHONE(String CUSTPHONE){
        this.CUSTPHONE = CUSTPHONE;
    }
    public String getCUSTADDR(){
        return CUSTADDR;
    }
    public String getCUSTPHONE(){
        return CUSTPHONE;
    }
    public String getCUSTNAME(){
        return CUSTNAME;
    }
    public String getCUSTID(){
        return CUSTID;
    }
    public static void PrintGuest() {
        System.out.println("==================");
        System.out.println("daftar nama tamu");
        System.out.println("==================");
    }
    public static void PrintGuest(ArrayList<EvenOrganiser>daftar_tamu){
        System.out.println("\n ==============Data GUEST===============");
        for(EvenOrganiser tamu : daftar_tamu){
            System.out.println("id\t:"+tamu.getCUSTID());
            System.out.println("nama\t"+tamu.getCUSTNAME());
            System.out.println("alamat\t"+tamu.getCUSTADDR());
            System.out.println("email\t"+tamu.getCUSTEMAIL());
            System.out.println("phone\t"+tamu.getCUSTPHONE()+"\n");
        }
    }
    public void cetakkartuevenorganiser(){
        System.out.println(this.getCUSTID());
        System.out.println(this.getCUSTNAME());
        System.out.println(this.getCUSTADDR());
        System.out.println(this.getCUSTEMAIL());
        System.out.println(this.getCUSTPHONE());
        System.out.println();
    }
    public EvenOrganiser (String CUSTID,String CUSTNAME,String CUSTADDR,String CUSTMAIL, String CUSTPHONE){
        this.CUSTID = CUSTID;
        this.CUSTNAME = CUSTNAME;
        this.CUSTADDR = CUSTADDR;
        this.CUSTEMAIL = CUSTMAIL;
        this.CUSTPHONE = CUSTPHONE;
    }
}
