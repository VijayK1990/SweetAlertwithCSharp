# SweetAlertwithCSharp
Sweet Alert Library written in C# mapping the JavaScript function

    protected void BtnSWAL_Success_Click(object sender, EventArgs e)
        {
            SweetAlert Swal = new SweetAlert()
            {
                Path = SweetAlertValues.NoPath,
                Title = SweetAlertValues.Title.Success,
                Message = "Operation completed",
                CssClass = SweetAlertValues.Css.Success,
                ExSwalRules = new ExtendedSweetAlertRules()
                {
                    ConfirmButtonColor = "Red"
                }
            };

            Page.ClientScript.RegisterStartupScript(GetType(), 
            JavascriptCodeIdentifier.SHOW_ALERT_DIALOG, SweetAlerter.EmbedSweetAlertCodeBlock(Swal), true);
        }
