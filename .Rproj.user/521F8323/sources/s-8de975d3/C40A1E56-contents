#' 按纽生成生成器界面
#'
#' @param colTitles  主页标题
#' @param widthRates 左右比例
#' @param func_left 左函数
#' @param func_right 右函数
#' @param tabTitle 标题
#' @param func_bottom  下面一栏
#'
#' @return 返回值
#' @import tsui
#' @export
#'
#' @examples
#' jhhrvcategoryTypeTableUI()

jhhrvcategoryTypeTableUI <- function(tabTitle ='业务类型表名埋点',
                    colTitles =c('操作区','显示区域'),
                    widthRates =c(4, 8),
                    func_left = buttoncategoryTypeTableUI_left,
                    func_right =buttoncategoryTypeTableUI_right
) {

  
  res = tsui::uiGen(tabTitle = tabTitle,colTitles =colTitles,widthRates = widthRates,func_left = func_left,func_right = func_right)
  return(res)
}


#' 操作区域
#'
#' @return 返回值
#' @export
#'
#' @examples
#' buttonUI_left()
buttoncategoryTypeTableUI_left <- function() {


  res <- tagList(

    shiny::actionButton(inputId = 'btn_view_categoryTypeTable' , label = '预览表单数据'),


  )
  return(res)

}





#' 预览区域
#'
#' @return 返回值
#' @export
#'
#' @examples
#' buttonUI_right()
buttoncategoryTypeTableUI_right <- function() {
  res <- tagList(
    tsui::uiScrollX(tsui::mdl_dataTable(id = 'view_data_categoryTypeTable', label = '出口'))
  )
  return(res)

}
