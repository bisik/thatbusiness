/* charger enable subfunction v0.1 */


void charger_enable()

bool x_ChargerEnableOutput;                             // Islemci uzerindeki ChargerEnableOutput pini
int i_ChargerType = 1;                                  //1=Canbus Haberlesme .... Farkli charger tiplerine gore yazilim esnetilebilecek. Default=1

if (i_ChargerType == 1)                                  //Canbus haberlesme kabiliyeti olan charger modeli icin bu kisim kullanilir.
{
	if (x_ChargingDeviceConnected && !(x_CriticalCondition || x_ChargingError) && !(x_ChargingFinished))
	{
		x_ChargerEnableOutput = true;
	}
	else
	{
		x_ChargerEnableOutput = false;
	}
}
