```java
import com.aliyuncs.DefaultAcsClient;
import com.aliyuncs.IAcsClient;
import com.aliyuncs.exceptions.ClientException;
import com.aliyuncs.exceptions.ServerException;
import com.aliyuncs.profile.DefaultProfile;
import com.google.gson.Gson;
import java.util.*;
import com.aliyuncs.smc.model.v20190601.*;

public class smcDemo {

    public static void main(String[] args) {
        DefaultProfile profile = DefaultProfile.getProfile("<RegionId>", "<AccessKey>", "<AccessSecret>");
        IAcsClient client = new DefaultAcsClient(profile);

        CreateReplicationJobRequest request = new CreateReplicationJobRequest();
        request.setSystemDiskSize(150);
        request.setSourceId("s-bp1ebo013cd21t4r****");

        try {
            CreateReplicationJobResponse response = client.getAcsResponse(request);
            System.out.println(new Gson().toJson(response));
        } catch (ServerException e) {
            e.printStackTrace();
        } catch (ClientException e) {
            System.out.println("ErrCode:" + e.getErrCode());
            System.out.println("ErrMsg:" + e.getErrMsg());
            System.out.println("RequestId:" + e.getRequestId());
        }
    }
}
```
