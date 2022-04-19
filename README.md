<!DOCTYPE HTML PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"><head>
    <title>Welcome </title>
    <link href="../css/pagelayout_2_0.css" type="text/css" rel="stylesheet" />
    <link href="../css/pageSchema_2_0.css" type="text/css" rel="stylesheet" />
    <link href="../css/schemaplus_styles.css" type="text/css" rel="stylesheet" />
    <link href="../css/billpay_styles.css" type="text/css" rel="stylesheet" />
    <link href="../css/splash_page_styles.css" type="text/css" rel="Stylesheet" />
	<link href="../css/royal_mod_layout.css" type="text/css" rel="Stylesheet" />
    <link href="../css/loan_action.css" type="text/css" rel="Stylesheet" />

    <script type="text/javascript" language="javascript" src="../js/jquery.js"></script>

    <script type="text/javascript" src="../includes/modules.txt">//datasource for writeMainMenu function</script>

    <script type="text/javascript" src="../includes/properties.txt">//datasource for properties</script>

    <script src="../js/basic_scripts.js" type="text/javascript"></script>

    <script src="../js/header_scripts.js" type="text/javascript"></script>

    <script src="../js/menu_scripts.js" type="text/javascript"></script>

    <script src="../js/content_scripts.js" type="text/javascript"></script>
	<script src="../js/loan_action.js" type="text/javascript"></script>

    <script language="javascript" src="../js/Tokenizer.js" type="text/javascript"></script>

    <script type="text/javascript" language="javascript">
		//variables used for isCheckedExternalTransfer Function
		var defaultMenu = "";
		var currentMenuTokens = defaultMenu.tokenize(";", "", true);
		var currentLoanTokens = defaultMenu.tokenize(";", "", true);
		//variables used for showMenuItem function to
		mainMenu = new Array();
		loanMenu = new Array();
		wireMenu = new Array();
		achMenu = new Array();	
		 
		 function ShowNoteVisibility()
		 {
		   if(showMenuItem('largereporting')!= '1' && showMenuItem('midreporting')!= '1') 
		   document.getElementById('Note').style.display = 'none';
		 }	
		 
		 function NavigateToSearchPage()
		 {
		  if(showMenuItem('largereporting') == '1')
		  location.href="../large_reporting/account_activity_search.html";
		  else if (showMenuItem('midreporting') == '1')
		  location.href="../mid_reporting/account_activity_search.html";
		 }
				
    </script>

    <style type="text/css">
        .modal-overlay
        {
            height: 120%;
        }
        .modal-window
        {
            top: 50%;
            left: 40%;
        }
		#cell_content_info,#cell_content_info_alt
		{
			border-radius:4px;
			-moz-border-radius:4px
		}
		
		ul
		{
		margin:0px;
		padding:0px;
		list-style-type:none
		}
    </style>
</head>
<body id="layout_body" onload="writeMainMenu('welcome');writeFavorites('favorites');
  								writeSavedReports('saved_reports');writeWelcomeAccounts('accountcontent');
								writeWelcomeCDAccounts('cdcontent');
								writeWelcomeInvestmentAccounts('investcontent');
  								writeWelcomeLoans('loancontent');checkLoanHeader('loanheader');checkCDAccountHeader('cdheader');checkInvestmentAccountHeader('investmentheader');ShowNoteVisibility();
  								writeWelcomeCard('cardcontent');checkCardHeader('cardheader');
								writeWelcomeRewards('rewardscontent'),checkRewardsHeader('rewardsheader');writeWelcomeDesa('desacontent'),checkDesaHeader('desaheader');GetQstringVal('../splash_pages/splash_page.html');writeCIS('cisheader'); return false; ">
    <table cellpadding="0" cellspacing="0" width="100%" height="100%" border="0">
        <tr>
            <td width="100%" colspan="3">
                <!-- ******************* -->
                <!--HEADER-->
                <!-- ******************* -->
                <div id="header_banner">
                    <table cellpadding="0" cellspacing="0" width="100%" align="center" border="0">
                        <tr>
                            <td class="header_banner_left" valign="middle" align="left">
                                <a href="#">

                                    <script type="text/javascript">writeHeaderLogo()</script>

                                </a>
                            </td>
                            <td class="header_banner_right" width="100%" valign="top" align="right">
                                <ul class="utilityLinks">
                                    <li class="normalUtilityLink"><a href="#" onclick="return false">Bank Home</a> </li>
                                    <li class="normalUtilityLink"><a href="javascript:openDisclosure('../includes/disclosure.html')">
                                        Disclosures</a> </li>
                                    <li class="normalUtilityLink"><a href="javascript:openHelp('../Help/modules_main/HelpPage.html')">
                                        Help</a> </li>
                                    <li class="lastUtilityLink"><a href="../index.html">Sign Off</a> </li>
                                </ul>
                                <span class="banner_product_text">

                                    <script type="text/javascript">writeProductName()</script>

                                </span>
                            </td>
                        </tr>
                    </table>
                </div>
                <!-- ******************* -->
                <!--END HEADER-->
                <!-- ******************* -->
                <!-- ******************* -->
                <!-- Main Menu -->
                <!-- ******************* -->
                <div id="welcome">
                </div>
              
                <!-- ******************* -->
                <!-- End Main Menu -->
                <!-- ******************* -->
            </td>
        </tr>
        <!-- from above the header -->
        <tr>
            <!-- ******************* -->
            <!-- Left Nav -->
            <!-- ******************* -->
            <td id="cell_menu_nav" valign="top" align="left" style="white-space: normal" width="185px"
                height="100%">
                <div id="favorites" class="divContentList" style="background: url('../images/newimages/left-gradient.png') repeat-x scroll 0 0 #FFFFFF;">
                </div>
                <div id="saved_reports">
                </div>
                <div>
                    <table cellpadding="0" cellspacing="0" width="100%" border="0">
                        <tr>
                            <td valign="top" width="100%">

                                <script type="text/javascript">writeLeftBanner()</script>

                            </td>
                        </tr>
                    </table>
                </div>
            </td>
            <!-- ******************* -->
            <!-- End Left Nav -->
            <!-- ******************* -->
            <!-- ******************* -->
            <!-- Main Content -->
            <!-- ******************* -->
            <td  valign="top" width="100%" height="100%" style="padding: 0px 8px 0px 8px;">
                <table  width="100%" height="100%" cellpadding="0" cellspacing="4" style="border:none; margin-top:12px">
                    <tr>
                        <td id="cell_content_content" width="100%" height="100%" valign="top" style="padding-right:30px">
                            <table cellpadding="0" cellspacing="2" width="90%">
                                <tr>
                                    <td id="cell_status_text" class="message_status">
                                        Welcome Annabelle Peaches.<br /><br />
                                  </td>
                                </tr>
                            </table>
                            <table cellpadding="0" cellspacing="2" width="90%">
                                <tr>
                                    <td id="cell_instruction" class="message_detail">
                                        Your last

                                        <script type="text/javascript">writeProductName()</script>

                                        sign on was

                                        <script type="text/javascript">theDateText(1)</script>

                                        at 02:38 PM ET.<br /><br />
                                    </td>
                                </tr>
                                <tr>
                                  <td  class="message_detail"><strong>Thank you for banking with us. We value your business.</strong></td>
                                </tr>
                            </table>
                            <table cellpadding="0" cellspacing="0" width="100%">
                              <tr>
                                    <td id="cell_content_area" width="100%">
                                        <div id="depositheader">
                                            <br>
                                            <br>
                                            <span class="subheader">Deposit Account Balances as of

                                                <script type="text/javascript">theDate(0)</script>

                                                <br>
                                                <hr />
                                                <span class="message_detail"><b>To view deposit account details, click the Account Number.</b>
                                                    Accounts are displayed in order of description. To change account descriptions,
                                                    go to <a href="../administration/account_admin.html" class="default">Account Administration</a>.
                                                </span></span>
                                            <br />
                                            <span class="message_detail" id="Note">
                                                <br />
                                                <!--Note: You have more accounts. To view more account information, go to&nbsp; <span
                                                    id="Reporting_Hyperlink"><a style="cursor: pointer" onclick="javascript:NavigateToSearchPage()"
                                                        class="default">Account Activity Criteria</a>. </span>--></span>
                                            <div id="accountcontent">
                                            </div>
                                           
                                          
                                        </div>
                                      
                                        <div id="cdheader" class="subheader"  >
                                            <br>
                                            <br>
                                          CD Account Balances as of

                                            <script type="text/javascript">theDate(1)</script>

                                        </div>
                                        
                                        <div id="cdcontent">
                                        </div>
                                        
                                      
                                        <div id="investmentheader" class="subheader" >
										<br/>
                                        <br/>
                                        Investment Account Balances as of

                                            <script type="text/javascript">theDate(1)</script>

                                        </div>
                                       
                                        <div id="investcontent">
                                        </div>
                                        <div id="loanheader" class="subheader" >
										<br>
                                        <br>
                                            Loan Account Summary as of

                                            <script type="text/javascript">theDate(0)</script>

                                        </div>
                                        
                                        <div id="loancontent">
                                        </div>
                                        
                                        <div id="cardheader" class="subheader" >
										<br>
                                        <br>
                                            Credit Card Account Summary as of

                                            <script type="text/javascript">theDate(1)</script>

                                        </div>
                                       
                                        <div id="cardcontent">
                                        </div>
										<div id="rewardsheader" class="subheader" style="display: block">
										<br/>
										<br/>
                                            Rewards Account Balances as of 

                                            <script type="text/javascript">theDate(0)</script>
											<div style="padding:8px 0px 8px 0px;"><hr align="left width=100%"></div>
											<span class="message_detail">To view rewards account details, click the Account Number.</span>
<br/><br/>
                                        </div>
                                        <div id="rewardscontent">
                                        </div>
                                        <div id="desaheader" class="subheader" >
										<br>
                                        
                                            Escrow Accounts Summary as of

                                            <script type="text/javascript">theDate(1)</script>

                                        </div>
                                       <br>
                                        <div id="desacontent">
                                        </div>
                                        
                                        
                                        <div id="cisheader" style="display:none" >
										
                                        </div>
                                       
                                       
                                        <br/><br/>
                                    </td>
                                </tr>
                            </table>
                        </td>
                    </tr>
                </table>
            </td>
            <!-- ******************* -->
            <!-- End Main Content -->
            <!-- ******************* -->
            <!-- ******************* -->
            <!-- Right Content -->
            <!-- ******************* -->
            <td class="cell_content_right" width="151px" valign="top" align="center">
                <div>
                    <div id="cell_content_info" style="width:100%;background-color:transparent;background: url('../images/newimages/left-gradient.png') repeat-x scroll 0 0 #FFFFFF;">
                        <div class="message_detail" align="left" style="padding: 5px;">
                            <p style="margin-bottom: 7pt; margin-top: 0pt;">
                                <b>Message Center</b></p>
                            <p style="margin-bottom: 6pt; margin-top: 0pt;">
                                <a class="default" href="../customer_support/received.html">New messages:</a> <b>12</b>
                            </p>
                            <p style="margin-bottom: 0pt; margin-top: 0pt;">
                                <nobr>Need Help? <a class="default" 
		        href="../customer_support/send_message.html">Contact Us
                                </a></p>
                        </div>
                    </div>
                    <br>
                    <div id="cell_content_info" style="background-color:transparent;width:100%">
                        <div class="message_detail" align="left" style="padding: 5px;">
                            <a class="default" href="../scheduled_requests/next_scheduled_requests.html">Next Scheduled
                                Requests</a>
                        </div>
                    </div>
                    <br>
                    <div id="cell_content_info_alt" class="message_detail" style="width:100%;">
                       <div class="message_detail" align="left" style="padding: 7px;"> 
                            <span style="white-space:normal">Remember to observe ACH holiday processing schedule.</span>
                        </div>
                    </div>
                    <br>
                    <div>
                        <div class="message_detail" align="center" style="padding_top: 25px; padding_left: 5px;
                            padding_bottom: 5px; padding_right: 5px">
                            <a href="#" onclick="return false">

                                <script type="text/javascript">writeGraph0()</script>

                            </a>
                            <br>
                            <span class="inactive_link">

                                <script type="text/javascript">getText0()</script>

                            </span>
                            <br>
                            <br>
                            <a href="#" onclick="return false">

                                <script type="text/javascript">writeGraph1()</script>

                            </a>
                            <br>
                            <span class="inactive_link">

                                <script type="text/javascript">getText1()</script>

                            </span>
                            <br>
                            <br>
                            <a href="#" onclick="return false">

                                <script type="text/javascript">writeGraph2()</script>

                            </a>
                            <br>
                            <span class="inactive_link" style="white-space:normal">

                                <script type="text/javascript">getText2()</script>

                            </span>	
                            <br>
                            <br>
                            <a href="#" onclick="return false">

                                <script type="text/javascript">writeGraph3()</script>

                            </a>
                            <br>
                            <span class="inactive_link">

                                <script type="text/javascript">getText3()</script>

                            </span>
                            <br>
                            <br>
                        </div>
                    </div>
                </div>
            </td>
            <!-- ******************* -->
            <!-- End Right Content -->
            <!-- ******************* -->
        </tr>
    </table>
</body>
</html>
