---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeviceManagement()
request_body.@odata_type = '#microsoft.graph.deviceManagement'

request_body.subscriptionstate(DeviceManagementSubscriptionState.Active('devicemanagementsubscriptionstate.active'))

additional_data = [
'device_protection_overview' => request_body = DeviceProtectionOverview()
		request_body.@odata_type = 'microsoft.graph.deviceProtectionOverview'

		request_body.TotalReportedDeviceCount = 8

		request_body.InactiveThreatAgentDeviceCount = 14

		request_body.UnknownStateThreatAgentDeviceCount = 2

		request_body.PendingSignatureUpdateDeviceCount = 1

		request_body.CleanDeviceCount = 0

		request_body.PendingFullScanDeviceCount = 10

		request_body.PendingRestartDeviceCount = 9

		request_body.PendingManualStepsDeviceCount = 13

		request_body.PendingOfflineScanDeviceCount = 13

		request_body.CriticalFailuresDeviceCount = 11

		request_body.PendingQuickScanDeviceCount = 11


request_body.device_protection_overview = deviceProtectionOverview

'windows_malware_overview' => request_body = WindowsMalwareOverview()
		request_body.@odata_type = 'microsoft.graph.windowsMalwareOverview'

		request_body.MalwareDetectedDeviceCount = 10

		request_body.TotalMalwareCount = 1

		request_body.TotalDistinctMalwareCount = 9

malware_state_summary1 = ()
		malware_state_summary1.@odata_type = 'microsoft.graph.windowsMalwareStateCount'

		malware_state_summary1.state = 'actionFailed'

		malware_state_summary1.DeviceCount = 11

		malware_state_summary1.MalwareDetectionCount = 5

		malware_state_summary1.DistinctMalwareCount = 4

		malware_state_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


malwareStateSummaryArray []= malwareStateSummary1;
request_body.malwarestatesummary(malwareStateSummaryArray)


malware_severity_summary1 = ()
	malware_severity_summary1.@odata_type = 'microsoft.graph.windowsMalwareSeverityCount'

	malware_severity_summary1.severity = 'low'

	malware_severity_summary1.MalwareDetectionCount = 5

	malware_severity_summary1.DistinctMalwareCount = 4

	malware_severity_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


malwareSeveritySummaryArray []= malwareSeveritySummary1;
request_body.malwareseveritysummary(malwareSeveritySummaryArray)


malware_execution_state_summary1 = ()
malware_execution_state_summary1.@odata_type = 'microsoft.graph.windowsMalwareExecutionStateCount'

malware_execution_state_summary1.execution_state = 'blocked'

malware_execution_state_summary1.DeviceCount = 11

malware_execution_state_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


malwareExecutionStateSummaryArray []= malwareExecutionStateSummary1;
request_body.malwareexecutionstatesummary(malwareExecutionStateSummaryArray)


malware_category_summary1 = ()
malware_category_summary1.@odata_type = 'microsoft.graph.windowsMalwareCategoryCount'

malware_category_summary1.category = 'adware'

malware_category_summary1.DeviceCount = 11

malware_category_summary1.ActiveMalwareDetectionCount = 11

malware_category_summary1.DistinctActiveMalwareCount = 10

malware_category_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


malwareCategorySummaryArray []= malwareCategorySummary1;
request_body.malwarecategorysummary(malwareCategorySummaryArray)


malware_name_summary1 = ()
malware_name_summary1.@odata_type = 'microsoft.graph.windowsMalwareNameCount'

malware_name_summary1.malware_identifier = 'Malware Identifier value'

malware_name_summary1.name = 'Name value'

malware_name_summary1.DeviceCount = 11

malware_name_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


malwareNameSummaryArray []= malwareNameSummary1;
request_body.malwarenamesummary(malwareNameSummaryArray)


os_versions_summary1 = ()
os_versions_summary1.@odata_type = 'microsoft.graph.osVersionCount'

os_versions_summary1.os_version = 'Os Version value'

os_versions_summary1.DeviceCount = 11

os_versions_summary1.last_update_date_time = '2016-12-31T23:58:21.6459442-08:00'


osVersionsSummaryArray []= osVersionsSummary1;
request_body.osversionssummary(osVersionsSummaryArray)



request_body.windows_malware_overview = windowsMalwareOverview

];
request_body.additional_data(additional_data)





result = await client.device_management.patch(request_body = request_body)


```