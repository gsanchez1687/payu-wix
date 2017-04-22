# payu-wix


Esta es la solucion para coloca el boton de PAYU en WIX sin que se desaparezca al dar clic.


la solucion que encontre fue quitar el input de la imagen .png, le agrege un input al final para crear el boton de forma mas natutal, el estilo del boton cree un css para simular.

quedaria de la siguiente forma. Los value se le colocar los que genera en su cuenta de payu.

            <form target="blank" method="post" action="https://gateway.payulatam.com/ppp-web-gateway/pb.zul" accept-charset="UTF-8">                                
                <input name="buttonId" type="hidden" value=""/>
                <input name="merchantId" type="hidden" value=""/>
                <input name="accountId" type="hidden" value=""/>
                <input name="description" type="hidden" value="Prueba"/>
                <input name="referenceCode" type="hidden" value=""/>
                <input name="amount" type="hidden" value=""/>
                <input name="tax" type="hidden" value="0"/>
                <input name="taxReturnBase" type="hidden" value="0"/>
                <input name="shipmentValue" value="0" type="hidden"/>
                <input name="currency" type="hidden" value=""/>
                <input name="lng" type="hidden" value="es"/>
                <input name="approvedResponseUrl" type="hidden" value=""/>
                <input name="declinedResponseUrl" type="hidden" value=""/>
                <input name="pendingResponseUrl" type="hidden" value=""/>
                <input name="paymentMethods" type="hidden" value=""/>
                <input name="displayShippingInformation" type="hidden" value="NO"/>
                <input name="sourceUrl" id="urlOrigen" value="" type="hidden"/>
                <input name="buttonType" value="SIMPLE" type="hidden"/>
                <input name="signature" value="" type="hidden"/>
                <input type="submit" class="btn" value="pagar con payU">
              </form>
              
              
             
