"phoneNumber":{
          "countryCode":"91",
          "number":"1111111111"
    },

    public class Customer {

    @Id
    private  final String username ;

    private  Name name ;
    private  String country ;
    private Date dateOfBirth ;

    private  String gender ;
    private Address address;

    private  PhoneNumber phoneNumber ;
    private final Date registrationDate;
    private int loyaltyPoints;
    private Boolean isKycVerified;
    private  Boolean isPhoneNumberVerified=false ;

}



@AllArgsConstructor
@NoArgsConstructor             
@Data
public class PhoneNumber {

   // @JsonProperty("countryCode")
    private  String countryCode ;
   // @JsonProperty("number")
    private String number;
}

org.springframework.core.convert.ConverterNotFoundException: No converter found capable of converting from type [java.lang.String] to type [com.bankify.customer.model.PhoneNumber]

 Servlet.service() for servlet [dispatcherServlet] in context with path [] threw exception [Request processing failed: org.springframework.core.convert.ConverterNotFoundException: No converter found capable of converting from type [java.lang.String] to type [com.bankify.customer.model.PhoneNumber]] with root cause 

