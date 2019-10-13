# Ethereum Vulnerable Smart Contract Benchmark
## Vulnerability type
We present a brief definition of the vulnerability here.
### Dangerous DelegateCall
The argument of delegatecall can be provide by msg.data.
### Freezing Ether 
Smart contracts can receive ether but cannot send ether except through delegatecall.
### Reentrancy
Nonreentrant function invoked in reentrant manner.
### Gasless Send
Send() triggers out of gas exception due to expensive fallback & sender keep ether wrongfully.	
### Exception Disorder
Inconsistent error propagation of low-level calls.
### Block Number Dependency
Relying Block Number to decide ether transfer.	
### Timestamp Dependency
Relying timestamp to decide ether transfer.	
## Folder structure
Each vulnerability directory contains at least three sub-folders: abis, bins, and sols, which store the contract's abi file, bin file, and sol file. The contents of these three folders are available to run the Contractfuzzer tool. In addition, each vulnerability directory will have a "*.list" file that records names of all the vulnerability contracts in this folder. For ease of reference, We list all names as follows by vulnerability type.
### Dangerous DelegateCall（7）
DSProxy<br>
RiskSharingToken<br>
WyvernDAOProxy<br>
MultiSigStub<br>
Parsec<br>
Ciphs<br>
CBToken<br>
### Freezing Ether （8）
AmIOnTheFork<br>
ClassicCheck<br>
DateTime<br>
DateTimeLib<br>
Math<br>
SafeMathLibExt<br>
TokenEventLib<br>
UintLib<br>
### Reentrancy（13）
BountyHunt<br>
ETH_VAULT<br>
Forwarder<br>
FunFairSale<br>
InkPublicPresale<br>
LZLCoin<br>
Payee<br>
PIGGY_BANK<br>
PowerCoin<br>
Private_accumaulation_fund<br>
PrivateBank<br>
PrivateDeposit<br>
ProxyCreationAndExecute<br>
### Gasless Send（17）
BetBuyer<br>
BigRisk<br>
BuyerFund<br>
CreditDepositBank<br>
CryptoChamps<br>
Dappster<br>
Doubly<br>
EtherConsole<br>
Etheramid<br>
Ethereum_twelve_bagger<br>
EthronTokenPonzi<br>
Fermat<br>
HFConditionalTransfer<br>
NumberBoard<br>
Reward<br>
SafeConditionalHFTransfer<br>
Soleau<br>
### Exception Disorder（38）
FarmCoinSale<br>
CrowdSalePreICO<br>
IPchainStandardToken<br>
Store<br>
FreeEth<br>
ReplaySafeSplit<br>
DepositBank<br>
BigRisk<br>
NexxusToken<br>
TokenBank<br>
PrayerCoin<br>
ChargCoinContract<br>
TranferInTwoPart<br>
SafeConditionalHFTransfer<br>
PassDao<br>
RewardEDProxy<br>
Ethereum_twelve_bagger<br>
MillionEther<br>
DeltaBalances<br>
MultiplicatorX4<br>
WhaleGiveaway1<br>
WhaleGiveaway2<br>
Reward<br>
CreditDepositBank<br>
EDProxy<br>
EDOGE<br>
Pie<br>
Caller<br>
Honey<br>
StackDepthLib<br>
Ethsplit<br>
RaisingToken<br>
HFConditionalTransfer<br>
Soleau<br>
HelpMeSave<br>
PonziUnlimited<br>
CoinContract<br>
TokenPurchase<br>
### Block Number Dependency（37）
APPToken<br>
Bagholder<br>
Bob<br>
Bombs<br>
CABCoinICO<br>
CHEXToken<br>
CompetitionStore<br>
CrowdsaleTokens<br>
CryptoDuels<br>
CryptoGoldStandardCoin<br>
CryptoPoosToken<br>
Cubic<br>
DIVXToken<br>
Dil<br>
DoubleOrNothingImpl<br>
FarmCoinSale<br>
FidgETHSpinner<br>
HashToken<br>
KeberuntunganAcak<br>
KiddyToys<br>
MUSCToken<br>
MoacToken<br>
NFTHouseGame<br>
NatCoinCrowdsale<br>
OurRoulette<br>
PreIcoCrowdsale<br>
Profit1000<br>
REPOExchange<br>
RandoCoin<br>
SCCsale<br>
STRIMToken<br>
SatoshiDice<br>
SmartBillions<br>
Videos<br>
WolkToken<br>
Wolker<br>
XCTCrowdSale<br>
### Timestamp Dependency（152）
LitmusCrowdsale<br>
LotteryAdmin<br>
CryptoCarsRent<br>
CTV<br>
EGLToken<br>
OZRealestatesToken<br>
CTNTokenSale<br>
ChargCoinContract<br>
CrowdSaleTRH<br>
NYX<br>
EXPERIMENTAL_ETH_AUCTION<br>
WaterCrowdsale<br>
BBDExchange<br>
AmbrosusSale<br>
ObizcoinCrowdsale<br>
Deposit<br>
RichestTakeAll<br>
IQNSecondPreICO<br>
CrowdsalePre<br>
SingularDTVLaunch<br>
EthTermDeposits<br>
IntermediateVault<br>
EthDickMeasuringGamev3<br>
Protocol108<br>
BitkomSale<br>
EternalWealth<br>
ChristmasClub<br>
BetterAuction<br>
BeatOrgTokenMainSale<br>
VentanaToken<br>
SpaceICOToken<br>
Dividend<br>
GraphenePowerToken<br>
XmasCoinCrowdsale<br>
IQNCrowdsale<br>
CTCToken<br>
PotPotato<br>
Billiontix<br>
ForecasterReward<br>
QuasacoinTokenCrowdsale<br>
CccTokenIco<br>
HODLerParadise<br>
DropletCrowdSale<br>
DEEX<br>
IAHCToken<br>
BlockFoodPreSale<br>
TimeCapsuleEvent<br>
PAXCHANGEICO<br>
EthCapsule<br>
AumICO<br>
ProvidencePresale<br>
HodlerInvestmentClub<br>
SpanCoin<br>
ChronosCore<br>
XgoldCrowdsale<br>
EtherGuess<br>
AngelCentralBank<br>
Who<br>
AcjCrowdsale<br>
JobeumPresale<br>
Bounty0xPresale<br>
ECHO<br>
KingOfTheHill<br>
EthereumHole<br>
NewCratePreSale<br>
LympoICO<br>
BouleICO<br>
DYLC_ERC20Token<br>
JoysoCrowdsale<br>
SnovCrowdsale<br>
ClaimableCrowdsale<br>
CandySale<br>
LudumToken<br>
BRANDCOIN<br>
ECT2Crowdsale2<br>
ElecSaleSmartContract<br>
TulipMania<br>
RaiseFundsForACause<br>
HodlSale<br>
MidnightCoin<br>
PreTGE<br>
VZTPresale<br>
EtherHell<br>
FabricTokenFundraiser<br>
HolyCoin<br>
BsPresale<br>
NYXAccount<br>
XPresale<br>
ECT2Crowdsale<br>
TrumpFullTermToken<br>
Freeze<br>
RaffleStrangeLoop<br>
ChangeableRateCrowdsale<br>
TopKing<br>
AtomicSwap<br>
KyberNetworkTokenSale<br>
ICOContract<br>
MoldCoin<br>
EthDickMeasuringGamev2<br>
IungoPresale<br>
EtherHellDeluxe<br>
RENTCoin<br>
ShareTokenSale<br>
EosPizzaSliceDonationraiser<br>
TUStoken<br>
Gelios<br>
Indicoin<br>
SimpleAuction<br>
CryptoBabyName<br>
ExtendedQuantstampSale<br>
BitGallery<br>
EthMultiplicator<br>
Loan<br>
EtherTower<br>
Lescovex<br>
FarmCoinSale<br>
KPRToken<br>
EthBtcSale<br>
EthDickMeasuringGame<br>
ChrisCoin<br>
ElectionsMarketSavingsBank<br>
EthBird<br>
EthKing<br>
CoinCrowdICO<br>
Countdown<br>
EtherDick<br>
CandyClaim<br>
DepositBank<br>
LooksCoin<br>
BriskCoin<br>
Bombs<br>
CryptoPoosToken<br>
ALTCrowdsale<br>
HodlContract<br>
HYIP<br>
BizPyramid<br>
BokkyPooBahsAutonomousRefundathonFacility<br>
IndaHashToken<br>
Bagholder<br>
Cryptoverse<br>
BillPokerPreICO<br>
Cajutel<br>
MallcoinCrowdSale<br>
CentraToken<br>
CashPokerProICO<br>
Aequitas<br>
BLOCKCHAIN_DEPOSIT_BETA<br>
BokkyPooBahsEtherRefundablePrize<br>
ListingsERC20<br>
Avalanche<br>
ArbiPreIco<br>
MarchMadness<br>